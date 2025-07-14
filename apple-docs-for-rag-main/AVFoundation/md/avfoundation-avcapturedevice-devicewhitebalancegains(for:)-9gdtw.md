

- AVFoundation
- AVCaptureDevice
-  deviceWhiteBalanceGains(for:) 

Instance Method

# deviceWhiteBalanceGains(for:)

Converts device-independent chromaticity values to device-specific white balance RGB gain values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
func deviceWhiteBalanceGains(for chromaticityValues: AVCaptureDevice.WhiteBalanceChromaticityValues) -> AVCaptureDevice.WhiteBalanceGains
```

## Parameters 

`chromaticityValues`  

The chromaticity values for which to get white balance RGB gain values.

## Return Value

A structure that contains device-specific RGB gain values.

## Discussion

This property specifies the current red, green, and blue gain values used for white balance. You can use the values to adjust color casts for a given scene.

Each channel supports values between `1.0` and -maxWhiteBalanceGain.

This property is key-value observable.

## See Also

### Performing Conversions

func chromaticityValues(for: AVCaptureDevice.WhiteBalanceGains) -> AVCaptureDevice.WhiteBalanceChromaticityValues

Converts device-specific white balance RGB gain values to device-independent chromaticity values.

func temperatureAndTintValues(for: AVCaptureDevice.WhiteBalanceGains) -> AVCaptureDevice.WhiteBalanceTemperatureAndTintValues

Converts device-specific white balance RGB gain values to device-independent temperature and tint values.

func deviceWhiteBalanceGains(for: AVCaptureDevice.WhiteBalanceTemperatureAndTintValues) -> AVCaptureDevice.WhiteBalanceGains

Converts device-independent temperature and tint values to device-specific white balance RGB gain values.

struct WhiteBalanceGains

A structure that defines RGB white balance gain values.

struct WhiteBalanceChromaticityValues

A structure that defines CIE 1931 xy chromaticity values.

struct WhiteBalanceTemperatureAndTintValues

A structure that defines temperature and tint values correlated to a white-balance color.

