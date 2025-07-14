

- Game Controller
- GCDevice
-  handlerQueue 

Instance Property

# handlerQueue

The dispatch queue that the framework uses to call element value change handlers.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var handlerQueue: dispatch_queue_t { get set }
```

**Required**

## Mentioned in 

Handling input events

## Discussion

The default queue is the main queue. Set this property to another queue to asynchronously call value change handlers (see GCControllerAxisInput, GCControllerButtonInput, GCControllerDirectionPad, and GCMotion). For example, if you handle input on another queue, set this property when you first access the input device.

## See Also

### Handling input

var physicalInputProfile: GCPhysicalInputProfile

The device’s physical input profile, such as a controller’s extended gamepad.

**Required**

Deprecated

