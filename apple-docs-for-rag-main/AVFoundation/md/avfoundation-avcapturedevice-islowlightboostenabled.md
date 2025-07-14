

- AVFoundation
- AVCaptureDevice
-  isLowLightBoostEnabled 

Instance Property

# isLowLightBoostEnabled

A Boolean value that indicates whether the capture device’s low light boost feature is in an enabled state.

iOS 6.0+iPadOS 6.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var isLowLightBoostEnabled: Bool { get }
```

## Discussion

The value of this property indicates whether the capture device currently enhancing images to improve quality due to low light conditions. When this property is true, the capture device has switched into a special mode in which it perceives more light in images.

This property is key-value observable.

## See Also

### Configuring Low Light Settings

var isLowLightBoostSupported: Bool

A Boolean value that indicates whether the capture device supports boosting images in low-light conditions.

var automaticallyEnablesLowLightBoostWhenAvailable: Bool

A Boolean value that indicates whether the capture device automatically switches to low-light boost mode when necessary.

