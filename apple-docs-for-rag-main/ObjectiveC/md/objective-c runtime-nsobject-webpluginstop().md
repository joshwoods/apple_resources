

- Objective-C Runtime
- NSObject
-  webPlugInStop() 

Instance Method

# webPlugInStop()

Tells the plug-in to stop normal operation.

macOS

``` source
func webPlugInStop()
```

## Discussion

This method may be called more than once, provided that the application has already called webPlugInInitialize() and that each call to this method is preceded by a call to webPlugInStart().

## See Also

### Controlling the Plug-in

func webPlugInDestroy()

Prepares the plug-in for deallocation.

func webPlugInInitialize()

Initializes the plug-in.

func webPlugInStart()

Tells the plug-in to start normal operation.

