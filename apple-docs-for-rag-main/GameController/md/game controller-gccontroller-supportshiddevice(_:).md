

- Game Controller
- GCController
-  supportsHIDDevice(\_:) 

Type Method

# supportsHIDDevice(\_:)

Returns a Boolean value that indicates whether the framework supports the specified human interface device.

macOS 11.0+

``` source
class func supportsHIDDevice(_ device: IOHIDDevice) -> Bool
```

## Parameters 

`device`  

A human interface input device.

## Return Value

true if the framework supports the device; otherwise, false.

## Discussion

If the Game Controller framework supports the input device, you can use the Game Controller APIs to interact with the device instead of the IOKit APIs.

## See Also

### Inspecting a controller

var isAttachedToDevice: Bool

A Boolean value that indicates whether the controller closely integrates with the device.

class var shouldMonitorBackgroundEvents: Bool

A Boolean value that indicates whether the app needs to respond to controller events when it isn’t the frontmost app.

