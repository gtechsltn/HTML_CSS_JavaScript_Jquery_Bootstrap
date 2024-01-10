# HTML, CSS, JavaScript, Jquery and Bootstrap
+ IIS
+ ASP.NET
+ HTML
+ CSS
+ JavaScript
+ Jquery
+ Bootstrap

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
+ applicationPool:"myAppPool"
+ site.name:"HTML_CSS_JavaScript_Jquery_Bootstrap"

## App Pool with with Specific Settings (.NET Framework)
%systemroot%\system32\inetsrv\APPCMD add apppool /name:myAppPool /managedRuntimeVersion:v4.0

## App Pool with with Specific Settings (.NET Core)
%systemroot%\system32\inetsrv\APPCMD add apppool /name:myAppPool /managedRuntimeVersion:""

## App Pool with Default Settings
%systemroot%\system32\inetsrv\APPCMD add apppool /name:myAppPool

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

defaultDocument in <system.webServer />

```
%systemroot%\system32\inetsrv\AppCmd.exe set config "HTML_CSS_JavaScript_Jquery_Bootstrap" /section:defaultDocument /enabled:true
```

# 6/ Directory Browse

directoryBrowse in <system.webServer />

```
%systemroot%\system32\inetsrv\AppCmd.exe set config "HTML_CSS_JavaScript_Jquery_Bootstrap" /section:directoryBrowse /enabled:true
```

# 7/ Change bindings
```
%systemroot%\system32\inetsrv\AppCmd.exe set site /site.name:"HTML_CSS_JavaScript_Jquery_Bootstrap" /+bindings.[protocol='http',bindingInformation='*:8389:']
```

# 8/ Start/Stop Site
```
%systemroot%\system32\inetsrv\AppCmd.exe start site /site.name:"HTML_CSS_JavaScript_Jquery_Bootstrap"
%systemroot%\system32\inetsrv\AppCmd.exe stop site /site.name:"HTML_CSS_JavaScript_Jquery_Bootstrap"
```

# 9/ Set config
```
%systemroot%\system32\inetsrv\AppCmd.exe set config "HTML_CSS_JavaScript_Jquery_Bootstrap" /section:defaultDocument /+files.[value='index.html;index.htm']
```
