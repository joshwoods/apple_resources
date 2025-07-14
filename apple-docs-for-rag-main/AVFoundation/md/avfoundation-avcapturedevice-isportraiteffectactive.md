

- AVFoundation
- AVCaptureDevice
-  isPortraitEffectActive 

Instance Property

# isPortraitEffectActive

A Boolean value that indicates whether the Portrait video effect is active on a device.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+

``` source
var isPortraitEffectActive: Bool { get }
```

## Discussion

When active, the device blurs the background, simulating a shallow depth of field effect. The device also limits the values of its activeVideoMinFrameDuration and activeVideoMaxFrameDuration to the value that the device format’s videoFrameRateRangeForPortraitEffect specifies.

When a capture device’s isPortraitEffectEnabled property value is true, it may also return true for this property, depending on whether it supports the feature in its current configuration.

This property is key-value observable.

## See Also

### Inspecting the Portrait Effect Settings

class var isPortraitEffectEnabled: Bool

A Boolean value that indicates whether the user enabled the Portrait video effect in Control Center.

