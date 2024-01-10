# HTML, CSS, JavaScript, Jquery and Bootstrap
+ Windows, IIS, ASP.NET, HTTP, XML
+ HTML, CSS, JavaScript, Jquery and Bootstrap

# HTTP
+ http://localhost:8389/

# Git
```
git clone https://github.com/gtechsltn/HTML_CSS_JavaScript_Jquery_Bootstrap.git
cd HTML_CSS_JavaScript_Jquery_Bootstrap
dotnet new gitignore
git checkout -b master
git push --set-upstream origin master
git add .
git commit -m "Add source to master"
git push
git checkout main
git pull
```

# Run Command Prompt as an Administrator Using the Run Dialog
```
md C:\inetpub\wwwroot\HTML_CSS_JavaScript_Jquery_Bootstrap
md C:\inetpub\wwwroot\HTML_CSS_JavaScript_Jquery_Bootstrap\Blog
%systemroot%\system32\inetsrv\APPCMD add apppool /name:myAppPool /managedRuntimeVersion:v4.0
%systemroot%\system32\inetsrv\APPCMD add site /name:mySiteName /bindings:http://*:80 /physicalpath:"C:\inetpub\wwwroot\HTML_CSS_JavaScript_Jquery_Bootstrap"
%systemroot%\system32\inetsrv\APPCMD add app /site.name:mySiteName /path:/blog /physicalPath:"C:\inetpub\wwwroot\HTML_CSS_JavaScript_Jquery_Bootstrap\Blog"
```

```
%systemroot%\system32\inetsrv\AppCmd.exe
```

# 1/ Add App Pool
+ applicationPool  : "myAppPool"
+ site.name        : "HTML_CSS_JavaScript_Jquery_Bootstrap"
+ app.name         : "blog"
```
/path:/blog
```

## App Pool with with Specific Settings (.NET Framework)

```
%systemroot%\system32\inetsrv\APPCMD add apppool /name:myAppPool /managedRuntimeVersion:v4.0
```

## App Pool with with Specific Settings (.NET Core)

```
%systemroot%\system32\inetsrv\APPCMD add apppool /name:myAppPool /managedRuntimeVersion:""
```

## App Pool with Default Settings

```
%systemroot%\system32\inetsrv\APPCMD add apppool /name:myAppPool
```

# 2/ Add Site

```
%systemroot%\system32\inetsrv\APPCMD add site /name:"HTML_CSS_JavaScript_Jquery_Bootstrap" /bindings:http://*:8989 /physicalpath:"C:\inetpub\wwwroot\HTML_CSS_JavaScript_Jquery_Bootstrap"
```

# 3/ Add App

```
%systemroot%\system32\inetsrv\APPCMD add app /site.name:"HTML_CSS_JavaScript_Jquery_Bootstrap" /path:/blog /physicalPath:"C:\inetpub\wwwroot\HTML_CSS_JavaScript_Jquery_Bootstrap\Blog"
```

# 4/ Assign or Change App Pool

```
%systemroot%\system32\inetsrv\APPCMD set site /site.name:"HTML_CSS_JavaScript_Jquery_Bootstrap" /[path='/'].applicationPool:myAppPool
```

# 5/ Default Document

<defaultDocument /> in <system.webServer />

```
%systemroot%\system32\inetsrv\AppCmd.exe set config "HTML_CSS_JavaScript_Jquery_Bootstrap" /section:defaultDocument /enabled:true
```

# 6/ Directory Browse

<directoryBrowse /> in <system.webServer />

```
%systemroot%\system32\inetsrv\AppCmd.exe set config "HTML_CSS_JavaScript_Jquery_Bootstrap" /section:directoryBrowse /enabled:true
```

# 7/ Change bindings

Step 1: STOP SITE

```
%systemroot%\system32\inetsrv\AppCmd.exe stop site /site.name:"HTML_CSS_JavaScript_Jquery_Bootstrap"
```

Step 2: Remove all bindings

```
%systemroot%\system32\inetsrv\AppCmd.exe set config -section:system.applicationHost/sites /-"[name='HTML_CSS_JavaScript_Jquery_Bootstrap'].bindings.[protocol='http',bindingInformation='*:8389:']" /commit:apphost
```

Step 3: Add a bindings

```
%systemroot%\system32\inetsrv\AppCmd.exe set site /site.name:"HTML_CSS_JavaScript_Jquery_Bootstrap" /+bindings.[protocol='http',bindingInformation='*:8389:']
```

Step 4: Other config

Classic .NET AppPool

```
%systemroot%\system32\inetsrv\AppCmd.exe set app "HTML_CSS_JavaScript_Jquery_Bootstrap/" /applicationPool:"Classic .NET AppPool"
```

Step 5: START SITE

```
%systemroot%\system32\inetsrv\AppCmd.exe start site /site.name:"HTML_CSS_JavaScript_Jquery_Bootstrap"
```

Step 6: Site > Browse

+ http://localhost:4200/
+ http://localhost:5000/
+ http://localhost:8080/
+ http://localhost:8389/
+ http://localhost:8383/
+ http://localhost:8989/

# 8/ Start/Stop Site

Start

```
%systemroot%\system32\inetsrv\AppCmd.exe start site /site.name:"HTML_CSS_JavaScript_Jquery_Bootstrap"
```

Stop

```
%systemroot%\system32\inetsrv\AppCmd.exe stop site /site.name:"HTML_CSS_JavaScript_Jquery_Bootstrap"
```


# 9/ Set config
```
%systemroot%\system32\inetsrv\AppCmd.exe set config "HTML_CSS_JavaScript_Jquery_Bootstrap" /section:defaultDocument /+files.[value='index.html;index.htm']
```

# Samples
+ https://www.geeksforgeeks.org/how-to-automatically-close-alerts-using-twitter-bootstrap/
