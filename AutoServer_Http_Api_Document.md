# AutoServer Http Api


### ShellController  (Shell Api)

------------

- Check Device is Rooted or Not,If Device is rooted,it will return true,else return false.
```xml
  http://{your device ip:port}/root
  
  (such as http://192.168.1.100:8080/root)
```

- Return your Device Resolution
```xml
  http://{your device ip:port}/size

  (such as http://192.168.1.100:8080/size)
```

- Execute shell code,and return result.
```xml
  http://{your device ip:port}/shell?cmd={your command}

  (such as http://192.168.1.100:8080/shell?cmd=echo autoserver)
```
```xml
   Return Format:
   
  "s:"+successMsg+" m:"+errorMsg+" r:"+result

  (successMsg is real result)
```

- Execute shell code with root permission,and return result.
```xml
  http://{your device ip:port}/shellr?cmd={your command}

  (such as http://192.168.1.100:8080/shell?cmd=echo autoserver)
```

------------

### ShellController  (Screenshot Api) (Request Root Permission)

- Screenshot your Device and return Image
```xml
  http://{your device ip:port}/jpg
  
  http://{your device ip:port}/png

  (such as http://192.168.1.100:8080/jpg)
```

------------

### ShellController  (Ui Xml Api) (Request Root Permission)

- return Xml of your device of screen, it will renturn screen.xml or screen.uix
```xml
  http://{your device ip:port}/uix
  
  http://{your device ip:port}/ui

  (such as http://192.168.1.100:8080/ui)
```

------------

### XmlChooserController (Xml Chooser Api) (Help you find bounds)
- return JSONObject List of the real time xml with your key and value(contains).
```xml
  http://{your device ip:port}/getnodelistbykeyvaluecontains?key={your key}&value={your value}

  (such as http://{your device ip:port}/getnodelistbykeyvaluecontains?key=text&value=Start Server)
```
```xml
   Return Format:
   
   JSONObject List
  
   (JSONObject include node's all information)
```

- return JSONObject List of the real time xml with your key and value(equal).
```xml
  http://{your device ip:port}/getnodelistbykeyvalue?key={your key}&value={your value}

  (such as http://{your device ip:port}/getnodelistbykeyvaluecontains?key=text&value=Start Server)
```
```xml
   Return Format:
   
   JSONObject List
  
   (JSONObject include node's all information)
```

- return Bounds List of the real time xml with your key and value(contains).
```xml
  http://{your device ip:port}/getboundsbykeyvaluecontains?key={your key}&value={your value}

  (such as http://{your device ip:port}/getboundsbykeyvaluecontains?key=text&value=Start Server)
```
```xml
   Return Format:
   
   Bounds(String) List
```

- return Bounds List of the real time xml with your key and value(equal).
```xml
  http://{your device ip:port}/getboundsbykeyvalue?key={your key}&value={your value}

  (such as http://{your device ip:port}/getboundsbykeyvalue?key=text&value=Start Server)
```
```xml
   Return Format:
   
   Bounds(String) List
```

- return the first of Node List of the real time xml with your key and value(equal).
```xml
  http://{your device ip:port}/getnodebykeyvalue?key={your key}&value={your value}

  (such as http://{your device ip:port}/getnodebykeyvalue?key=text&value=Start Server)
```
```xml
   Return Format:
   
   the first of Node List
```
- return the first of Node List of the real time xml with your key and value(contains).
```xml
  http://{your device ip:port}/getnodebykeyvaluecontains?key={your key}&value={your value}

  (such as http://{your device ip:port}/getnodebykeyvaluecontains?key=text&value=Start Server)
```
```xml
   Return Format:
   
   the first of Node List
```
- return the first bounds of Node List of the real time xml with your key and value(contains).
```xml
  http://{your device ip:port}/getboundbykeyvaluecontains?key={your key}&value={your value}

  (such as http://{your device ip:port}/getboundbykeyvaluecontains?key=text&value=Start Server)
```
```xml
   Return Format:
   
   bounds(String)
```
- return the first bounds of Node List of the real time xml with your key and value(equal).
```xml
  http://{your device ip:port}/getboundbykeyvalue?key={your key}&value={your value}

  (such as http://{your device ip:port}/getboundbykeyvalue?key=text&value=Start Server)
```
```xml
   Return Format:
   
   bounds(String)
```
------------

### Contact Me

mr3317952@gmail.com
