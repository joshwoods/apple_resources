

- Objective-C Runtime
- NSObject
-  objectForWebScript 

Instance Property

# objectForWebScript

Returns an object that exposes the plug-in’s scripting interface.

macOS

``` source
var objectForWebScript: Any! { get }
```

## Return Value

An object representing the plug-in’s scripting interface.

## Discussion

The methods of the object are exposed to the script environment. Messages sent to the returned object will be invoked in the scripting environment. See the WebScripting Protocol Reference informal protocol for more details.

