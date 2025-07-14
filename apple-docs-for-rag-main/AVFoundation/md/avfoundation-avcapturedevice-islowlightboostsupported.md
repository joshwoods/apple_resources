

- AVFoundation
- AVCaptureDevice
-  isLowLightBoostSupported 

Instance Property

# isLowLightBoostSupported

A Boolean value that indicates whether the capture device supports boosting images in low-light conditions.

iOS 6.0+iPadOS 6.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var isLowLightBoostSupported: Bool { get }
```

## Discussion

You can set the capture device’s automaticallyEnablesLowLightBoostWhenAvailable property only if this property is true.

This property is key-value observable.

## See Also

### Configuring Low Light Settings

var isLowLightBoostEnabled: Bool

A Boolean value that indicates whether the capture device’s low light boost feature is in an enabled state.

var automaticallyEnablesLowLightBoostWhenAvailable: Bool

A Boolean value that indicates whether the capture device automatically switches to low-light boost mode when necessary.

