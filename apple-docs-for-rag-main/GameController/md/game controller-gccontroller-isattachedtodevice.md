

- Game Controller
- GCController
-  isAttachedToDevice 

Instance Property

# isAttachedToDevice

A Boolean value that indicates whether the controller closely integrates with the device.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var isAttachedToDevice: Bool { get }
```

## Discussion

If true, the controller may be formfitting or otherwise closely attach to the device so that the player can interact simultaneously with the controller and the device. If false, the controller doesn’t have an attachment to the device.

## See Also

### Inspecting a controller

class func supportsHIDDevice(IOHIDDevice) -> Bool

Returns a Boolean value that indicates whether the framework supports the specified human interface device.

class var shouldMonitorBackgroundEvents: Bool

A Boolean value that indicates whether the app needs to respond to controller events when it isn’t the frontmost app.

