

- Objective-C Runtime
- NSObject
-  webPlugInInitialize() 

Instance Method

# webPlugInInitialize()

Initializes the plug-in.

macOS

``` source
func webPlugInInitialize()
```

## Discussion

Tells the plug-in to perform one-time initialization. This method must be called only once per instance of the plug-in object, before any other methods in the protocol are called.

## See Also

### Controlling the Plug-in

func webPlugInDestroy()

Prepares the plug-in for deallocation.

func webPlugInStart()

Tells the plug-in to start normal operation.

func webPlugInStop()

Tells the plug-in to stop normal operation.

