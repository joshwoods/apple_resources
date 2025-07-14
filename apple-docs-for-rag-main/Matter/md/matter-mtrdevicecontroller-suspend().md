

- Matter
- MTRDeviceController
-  suspend() 

Instance Method

# suspend()

Suspend the controller. This will attempt to stop all network traffic associated with the controller. The controller will remain suspended until it is resumed.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+tvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
func suspend()
```

## Discussion

Suspending an already-suspended controller has no effect.

