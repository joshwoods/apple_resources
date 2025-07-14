

- Objective-C Runtime
- NSObject
-  webPlugInDestroy() 

Instance Method

# webPlugInDestroy()

Prepares the plug-in for deallocation.

macOS

``` source
func webPlugInDestroy()
```

## Discussion

Typically, this method frees the memory and other resources used by the plug-in. For example, if the plug-in had a copy of a WebPlugInContainer object, this method should relinquish ownership of that object. Do not send any other messages to the plug-in after invoking this method, because calling this method destroys the plug-in. No other methods in this interface may be called after the application has called this method.

## See Also

### Controlling the Plug-in

func webPlugInInitialize()

Initializes the plug-in.

func webPlugInStart()

Tells the plug-in to start normal operation.

func webPlugInStop()

Tells the plug-in to stop normal operation.

