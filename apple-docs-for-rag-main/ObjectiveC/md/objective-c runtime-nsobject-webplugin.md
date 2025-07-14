

- Objective-C Runtime
- NSObject
-  WebPlugIn 

API Collection

# WebPlugIn

The `WebPlugIn` informal protocol defines methods that enable interaction between an application using the WebKit framework and any WebKit-based plug-ins it may use.

## Topics

### Accessing the Scripting Environment

var objectForWebScript: Any!

Returns an object that exposes the plug-in’s scripting interface.

### Using Plug-in State Information

func webPlugInSetIsSelected(Bool)

Controls plug-in behavior based on its selection.

### Controlling the Plug-in

func webPlugInDestroy()

Prepares the plug-in for deallocation.

func webPlugInInitialize()

Initializes the plug-in.

func webPlugInStart()

Tells the plug-in to start normal operation.

func webPlugInStop()

Tells the plug-in to stop normal operation.

### Main resource messages

func webPlugInMainResourceDidFailWithError((any Error)!)

Invoked when an error occurs loading the main resource.

func webPlugInMainResourceDidFinishLoading()

Invoked when the connection successfully finishes loading data.

func webPlugInMainResourceDidReceive(Data!)

Invoked when the connection loads data incrementally.

func webPlugInMainResourceDidReceive(URLResponse!)

Invoked when the connection receives sufficient data to construct the URL response for its request.

## See Also

### Interacting with Web Plug-ins

WebPlugInContainer

`WebPlugInContainer` is an informal protocol that enables a plug-in to send messages to the application.

