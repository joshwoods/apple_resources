

- AVFoundation
- AVCaptureDevice
-  AVCaptureDevice.WhiteBalanceGains 

Structure

# AVCaptureDevice.WhiteBalanceGains

A structure that defines RGB white balance gain values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
struct WhiteBalanceGains
```

## Topics

### Creating White Balance Gains

init()

The default initializer for white balance gains.

init(redGain: Float, greenGain: Float, blueGain: Float)

Initializes a white balance gain from its red, green, and blue gain components.

### Isolating Gain by Color Channel

var blueGain: Float

The blue gain component of the white balance value.

var greenGain: Float

The green gain component of the white balance value.

var redGain: Float

The red gain component of the white balance value.

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

struct WhiteBalanceChromaticityValues

A structure that defines CIE 1931 xy chromaticity values.

struct WhiteBalanceTemperatureAndTintValues

A structure that defines temperature and tint values correlated to a white-balance color.

