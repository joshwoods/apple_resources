

- AVFoundation
- AVCaptureDevice
-  AVCaptureDevice.WhiteBalanceTemperatureAndTintValues 

Structure

# AVCaptureDevice.WhiteBalanceTemperatureAndTintValues

A structure that defines temperature and tint values correlated to a white-balance color.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
struct WhiteBalanceTemperatureAndTintValues
```

## Topics

### Creating Temperature and Tint Values

init()

Creates a default value.

init(temperature: Float, tint: Float)

Creates a structure with a white balance temperature and tint.

### Inspecting the Values

var temperature: Float

The white balance color correlated temperature in kelvin.

var tint: Float

The white balance tint value in the range of `-150.0` through `+150.0`.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Performing Conversions

func chromaticityValues(for: AVCaptureDevice.WhiteBalanceGains) -> AVCaptureDevice.WhiteBalanceChromaticityValues

Converts device-specific white balance RGB gain values to device-independent chromaticity values.

func temperatureAndTintValues(for: AVCaptureDevice.WhiteBalanceGains) -> AVCaptureDevice.WhiteBalanceTemperatureAndTintValues

Converts device-specific white balance RGB gain values to device-independent temperature and tint values.

func deviceWhiteBalanceGains(for: AVCaptureDevice.WhiteBalanceChromaticityValues) -> AVCaptureDevice.WhiteBalanceGains

Converts device-independent chromaticity values to device-specific white balance RGB gain values.

func deviceWhiteBalanceGains(for: AVCaptureDevice.WhiteBalanceTemperatureAndTintValues) -> AVCaptureDevice.WhiteBalanceGains

Converts device-independent temperature and tint values to device-specific white balance RGB gain values.

struct WhiteBalanceGains

A structure that defines RGB white balance gain values.

struct WhiteBalanceChromaticityValues

A structure that defines CIE 1931 xy chromaticity values.

