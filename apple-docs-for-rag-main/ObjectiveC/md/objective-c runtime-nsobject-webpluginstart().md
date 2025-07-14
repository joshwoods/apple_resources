

- Objective-C Runtime
- NSObject
-  webPlugInStart() 

Instance Method

# webPlugInStart()

Tells the plug-in to start normal operation.

macOS

``` source
func webPlugInStart()
```

## Discussion

The plug-in usually begins its primary task (such as drawing, playing sounds, or animating) in this method. This method may be called more than once, provided that the application has already called webPlugInInitialize() and that each call to this method is followed later by a call to webPlugInStop().

## See Also

### Controlling the Plug-in

func webPlugInDestroy()

Prepares the plug-in for deallocation.

func webPlugInInitialize()

Initializes the plug-in.

func webPlugInStop()

Tells the plug-in to stop normal operation.

