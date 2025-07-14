

- Media Accessibility
-  MADimFlashingLightsEnabled() 

Function

# MADimFlashingLightsEnabled()

Returns a Boolean value that indicates whether the flashing lights setting is enabled on the device.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+

``` source
func MADimFlashingLightsEnabled() -> Bool
```

## See Also

### Dim flashing lights

Responding to changes in the flashing lights setting

Adjust your UI when a person chooses to dim flashing lights on their Apple device.

let kMADimFlashingLightsChangedNotification: CFString

A notification that posts when a person changes the flashing lights setting on the device.

class MAFlashingLightsProcessor

A class that processes a framebuffer object to detect and dim sequences of flashing lights.

