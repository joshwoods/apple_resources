

- AVFoundation
- AVCaptureDevice
-  deviceWhiteBalanceGains(for:) 

Instance Method

# deviceWhiteBalanceGains(for:)

Converts device-independent temperature and tint values to device-specific white balance RGB gain values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
func deviceWhiteBalanceGains(for tempAndTintValues: AVCaptureDevice.WhiteBalanceTemperatureAndTintValues) -> AVCaptureDevice.WhiteBalanceGains
```

## Parameters 

`tempAndTintValues`  

An AVCaptureDevice.WhiteBalanceTemperatureAndTintValues structure containing the temperature and tint values.

## Return Value

A fully populated AVCaptureDevice.WhiteBalanceGains structure containing device-specific RGB gain values.

## Discussion

Call this method to convert device-independent temperature and tint values to device-specific RGB white balance gain values.

You may pass any temperature and tint values and corresponding white balance gains will be produced. Note, though, that some temperature and tint combinations yield out-of-range device RGB values that will cause an exception to be thrown if passed directly to setWhiteBalanceModeLocked(with:completionHandler:). Be sure to verify that the red, green, and blue gain values are within the range of \[`1.0` - maxWhiteBalanceGain\].

## See Also

### Performing Conversions

func chromaticityValues(for: AVCaptureDevice.WhiteBalanceGains) -> AVCaptureDevice.WhiteBalanceChromaticityValues

Converts device-specific white balance RGB gain values to device-independent chromaticity values.

func temperatureAndTintValues(for: AVCaptureDevice.WhiteBalanceGains) -> AVCaptureDevice.WhiteBalanceTemperatureAndTintValues

Converts device-specific white balance RGB gain values to device-independent temperature and tint values.

func deviceWhiteBalanceGains(for: AVCaptureDevice.WhiteBalanceChromaticityValues) -> AVCaptureDevice.WhiteBalanceGains

Converts device-independent chromaticity values to device-specific white balance RGB gain values.

struct WhiteBalanceGains

A structure that defines RGB white balance gain values.

struct WhiteBalanceChromaticityValues

A structure that defines CIE 1931 xy chromaticity values.

struct WhiteBalanceTemperatureAndTintValues

A structure that defines temperature and tint values correlated to a white-balance color.

