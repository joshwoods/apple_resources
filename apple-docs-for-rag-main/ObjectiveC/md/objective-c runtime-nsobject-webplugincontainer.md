

- Objective-C Runtime
- NSObject
-  WebPlugInContainer 

API Collection

# WebPlugInContainer

`WebPlugInContainer` is an informal protocol that enables a plug-in to send messages to the application.

## Topics

### Performing actions on the enclosing container

func webPlugInContainerLoad(URLRequest!, inFrame: String!)

Loads a URL into a web frame.

func webPlugInContainerShowStatus(String!)

Tells the container to show a status message.

### Obtaining information about the container

var webFrame: WebFrame!

Returns the `WebFrame` that contains the plug-in.

var webPlugInContainerSelectionColor: NSColor!

Returns the plug-in selection color.

## See Also

### Related Documentation

WebKit Objective-C Programming Guide

### Interacting with Web Plug-ins

WebPlugIn

The `WebPlugIn` informal protocol defines methods that enable interaction between an application using the WebKit framework and any WebKit-based plug-ins it may use.

