

- AVFoundation
- AVCaptureDevice
-  temperatureAndTintValues(for:) 

Instance Method

# temperatureAndTintValues(for:)

Converts device-specific white balance RGB gain values to device-independent temperature and tint values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
func temperatureAndTintValues(for whiteBalanceGains: AVCaptureDevice.WhiteBalanceGains) -> AVCaptureDevice.WhiteBalanceTemperatureAndTintValues
```

## Parameters 

`whiteBalanceGains`  

The white balance gain values. You can’t specify a value of currentWhiteBalanceGains.

## Return Value

A structure that contains device-independent values.

## Discussion

Each change in the structure supports values between `1.0` and maxWhiteBalanceGain. This method throws an exception if you specify an unsupported value.

## See Also

### Performing Conversions

func chromaticityValues(for: AVCaptureDevice.WhiteBalanceGains) -> AVCaptureDevice.WhiteBalanceChromaticityValues

Converts device-specific white balance RGB gain values to device-independent chromaticity values.

func deviceWhiteBalanceGains(for: AVCaptureDevice.WhiteBalanceChromaticityValues) -> AVCaptureDevice.WhiteBalanceGains

Converts device-independent chromaticity values to device-specific white balance RGB gain values.

func deviceWhiteBalanceGains(for: AVCaptureDevice.WhiteBalanceTemperatureAndTintValues) -> AVCaptureDevice.WhiteBalanceGains

Converts device-independent temperature and tint values to device-specific white balance RGB gain values.

struct WhiteBalanceGains

A structure that defines RGB white balance gain values.

struct WhiteBalanceChromaticityValues

A structure that defines CIE 1931 xy chromaticity values.

struct WhiteBalanceTemperatureAndTintValues

A structure that defines temperature and tint values correlated to a white-balance color.

