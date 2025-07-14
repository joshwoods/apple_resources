

- AVFoundation
- AVCaptureDevice
-  AVCaptureDevice.WhiteBalanceChromaticityValues 

Structure

# AVCaptureDevice.WhiteBalanceChromaticityValues

A structure that defines CIE 1931 xy chromaticity values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
struct WhiteBalanceChromaticityValues
```

## Topics

### Creating Chromaticity Values

init()

Creates a structure for white balance chromaticity values.

init(x: Float, y: Float)

Creates a structure for white balance chromaticity values from its x and y coordinates.

### Inspecting the Values

var x: Float

The x component of the CIE 1931 chromaticity value.

var y: Float

The y component of the CIE 1931 chromaticity value.

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

struct WhiteBalanceTemperatureAndTintValues

A structure that defines temperature and tint values correlated to a white-balance color.

