# HTML, CSS, JavaScript, Jquery and Bootstrap
+ Windows, IIS, ASP.NET, HTTP, XML, JSON
+ HTML, CSS, JavaScript, Jquery and Bootstrap

## Versions
+ **jQuery** version 3.7.1
+ **Handlebars.js** version 4.7.8
  + npm view handlebars version --json
  + http://www.alpacajs.org/tutorial.html
+ **Bootstrap** version 3.4.1
+ Font Awesome version 4.7.0
+ **Moment.js** version 2.29.1
  + https://cdnjs.cloudflare.com/ajax/libs/moment.js
  + https://cdnjs.cloudflare.com/ajax/libs/moment.js/2.30.1/moment.min.js
  + https://cdnjs.cloudflare.com/ajax/libs/moment.js/2.30.1/moment-with-locales.min.js
  + https://cdnjs.cloudflare.com/ajax/libs/moment.js/2.30.1/locale/vi.min.js
  
+ Eonasdan Bootstrap Datetimepicker version 4.17.47
  + Bootstrap 3 Datetimepicker CSS
  + Moment JS
  + Bootstrap 3 Datetimepicker JS
+ **Alpaca.js** version 1.5.27
  + npm view alpaca version --json
  + Alpaca - Easy Forms for jQuery
  + Easily create forms for your web site using jQuery, Bootstrap and JSON Schema.
  + http://www.alpacajs.org/
  + http://www.alpacajs.org/documentation.html
  + http://www.alpacajs.org/examples.html
  + This example loads data, schema and options parameters through ajax calls.
  + http://www.alpacajs.org/demos/bootstrap/multi-column-layouts/index.html
  + Alpaca - JSON Forms for jQuery and Bootstrap
  + https://github.com/gitana/alpaca
  + https://cdnjs.cloudflare.com/ajax/libs/handlebars.js/<version>/handlebars.js
  + https://cdn.jsdelivr.net/npm/alpaca@<version>/dist/alpaca/bootstrap/alpaca.min.js
  + https://cdn.jsdelivr.net/npm/alpaca@<version>/dist/alpaca/bootstrap/alpaca.min.css
+ **Highlight.js** version 11.9.0
  + npm view highlight.js version --json
+ **Ember.js** version 5.5.0
  + npm view ember-cli version --json
  + npm view ember-data version --json
  + npm view ember-source version --json

```
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css" />
<link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons" />
<link rel='stylesheet' href='https://fonts.googleapis.com/css?family=Roboto|Pacifico' />
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/3.4.1/css/bootstrap.min.css" />
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/alpaca@1.5.27/dist/alpaca/bootstrap/alpaca.min.css" />
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/eonasdan-bootstrap-datetimepicker/4.17.47/css/bootstrap-datetimepicker.min.css" />
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.7.1/jquery.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/handlebars.js/4.7.8/handlebars.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/3.4.1/js/bootstrap.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/moment.js/2.29.1/moment-with-locales.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/eonasdan-bootstrap-datetimepicker/4.17.47/js/bootstrap-datetimepicker.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/alpaca@1.5.27/dist/alpaca/bootstrap/alpaca.min.js"></script>
```

# CDN (Libraries)
+ https://cdnjs.com/libraries/jquery
+ https://cdnjs.com/libraries/handlebars.js
+ https://cdnjs.com/libraries/twitter-bootstrap
+ https://cdnjs.com/libraries/font-awesome
+ https://cdnjs.com/libraries/eonasdan-bootstrap-datetimepicker
+ https://cdnjs.com/libraries/bootstrap
+ https://cdnjs.com/libraries/bootstrap-datepicker
+ https://cdnjs.com/libraries/bootstrap-table
+ https://cdnjs.com/libraries/bootstrap-fileinput
+ https://cdnjs.com/libraries/bootstrap-select
+ https://cdnjs.com/libraries/bootstrap-multiselect
+ https://cdnjs.com/libraries/moment.js
+ https://cdnjs.com/libraries/highlight.js
+ https://cdnjs.com/libraries/alpaca
+ https://cdnjs.com/libraries/select2
+ https://cdnjs.com/libraries/datatables

### HTTP
+ <a href="http://localhost:8389/" target="_blank">http://localhost:8389/</a>
+ <a href="https://github.com/gtechsltn/HTML_CSS_JavaScript_Jquery_Bootstrap/blob/main/src/index.html" target="_blank">index.html</a>
+ <a href="https://github.com/gtechsltn/HTML_CSS_JavaScript_Jquery_Bootstrap/blob/main/src/index.html" target="_blank">web.config</a>

### Alpaca and Alpaca Forms
+ Alpaca - JSON Forms for jQuery and Bootstrap
+ Alpaca Forms - Easy Forms for jQuery
+ https://emberobserver.com/categories/forms
+ https://toddjordan.github.io/ember-cli-dynamic-forms/
+ https://stackoverflow.com/questions/60782452/alpaca-is-there-a-form-onready
+ https://fenixrepo.fao.org/cdn/js/alpaca/1.5.17/dist/alpaca/jsdoc/index.html
+ Alpaca WordPress Theme Documentation
+ https://www.loftocean.com/alpaca-doc/documentation.html

### Git
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

### Run Command Prompt as an Administrator Using the Run Dialog
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

## 1/ Add App Pool
+ applicationPool  : "myAppPool"
+ site.name        : "HTML_CSS_JavaScript_Jquery_Bootstrap"
+ app.name         : "blog"
```
/path:/blog
```

#### App Pool with with Specific Settings (.NET Framework)

```
%systemroot%\system32\inetsrv\APPCMD add apppool /name:myAppPool /managedRuntimeVersion:v4.0
```

#### App Pool with with Specific Settings (.NET Core)

```
%systemroot%\system32\inetsrv\APPCMD add apppool /name:myAppPool /managedRuntimeVersion:""
```

#### App Pool with Default Settings

```
%systemroot%\system32\inetsrv\APPCMD add apppool /name:myAppPool
```

## 2/ Add Site

```
%systemroot%\system32\inetsrv\APPCMD add site /name:"HTML_CSS_JavaScript_Jquery_Bootstrap" /bindings:http://*:8989 /physicalpath:"C:\inetpub\wwwroot\HTML_CSS_JavaScript_Jquery_Bootstrap"
```

## 3/ Add App

```
%systemroot%\system32\inetsrv\APPCMD add app /site.name:"HTML_CSS_JavaScript_Jquery_Bootstrap" /path:/blog /physicalPath:"C:\inetpub\wwwroot\HTML_CSS_JavaScript_Jquery_Bootstrap\Blog"
```

## 4/ Change App Pool

```
%systemroot%\system32\inetsrv\APPCMD set site /site.name:"HTML_CSS_JavaScript_Jquery_Bootstrap" /[path='/'].applicationPool:myAppPool
```

## 5/ Default Document

<defaultDocument /> in <system.webServer />

```
%systemroot%\system32\inetsrv\AppCmd.exe set config "HTML_CSS_JavaScript_Jquery_Bootstrap" /section:defaultDocument /enabled:true
```

## 6/ Directory Browse

<directoryBrowse /> in <system.webServer />

```
%systemroot%\system32\inetsrv\AppCmd.exe set config "HTML_CSS_JavaScript_Jquery_Bootstrap" /section:directoryBrowse /enabled:true
```

## 7/ Change bindings

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
+ http://localhost:8389/

## 8/ Start Site and Stop Site

Start

```
%systemroot%\system32\inetsrv\AppCmd.exe start site /site.name:"HTML_CSS_JavaScript_Jquery_Bootstrap"
```

Stop

```
%systemroot%\system32\inetsrv\AppCmd.exe stop site /site.name:"HTML_CSS_JavaScript_Jquery_Bootstrap"
```


## 9/ Set config

SET defaultDocument: index.html

```
%systemroot%\system32\inetsrv\AppCmd.exe set config "HTML_CSS_JavaScript_Jquery_Bootstrap" /section:defaultDocument /+files.[value='index.html;index.htm']
```

SET physicalPath: D:\gtechsltn\HTML_CSS_JavaScript_Jquery_Bootstrap\src

```
%systemroot%\system32\inetsrv\AppCmd.exe set vdir "HTML_CSS_JavaScript_Jquery_Bootstrap/" -physicalPath:"D:\gtechsltn\HTML_CSS_JavaScript_Jquery_Bootstrap\src"
```


## 10/ Samples
+ https://www.geeksforgeeks.org/how-to-automatically-close-alerts-using-twitter-bootstrap/
+ https://www.geeksforgeeks.org/how-to-place-font-awesome-icon-to-input-field/
+ https://www.geeksforgeeks.org/css-to-put-icon-inside-an-input-element-in-a-form/
+ https://www.w3schools.com/bootstrap/tryit.asp?filename=trybs_grid_stacked_to_hor&stacked=v
+ https://stackoverflow.com/questions/45029302/bootstrap-make-last-row-stretch-to-the-remaining-height-and-stick-text-to-butto
+ https://jsfiddle.net/ksiabani/wsvc4j31/
+ https://getdatepicker.com/4/
+ http://www.alpacajs.org/
+ http://www.alpacajs.org/tutorial.html
+ https://github.com/gitana/alpaca
+ http://www.alpacajs.org/docs/api/serialization.html
+ https://stackoverflow.com/questions/23483550/generate-forms-on-the-fly-using-emberjs-and-json-schema
+ https://www.copahost.com/blog/bootstrap-cdn-include/
