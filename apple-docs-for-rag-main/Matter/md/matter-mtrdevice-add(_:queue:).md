

- Matter
- MTRDevice
-  add(\_:queue:) 

Instance Method

# add(\_:queue:)

Adds a delegate to receive asynchronous callbacks about the device.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func add(
    _ delegate: any MTRDeviceDelegate,
    queue: dispatch_queue_t
)
```

## Discussion

The delegate will be called on the provided queue, for attribute reports, event reports, and device state changes.

MTRDevice holds a weak reference to the delegate object.

