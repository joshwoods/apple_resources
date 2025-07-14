

- SensorKit
- SRAmbientLightSample
-  SRAmbientLightSample.SensorPlacement 

Enumeration

# SRAmbientLightSample.SensorPlacement

Directional values that describe light-source location with respect to the sensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
enum SensorPlacement
```

## Topics

### Placement configurations

case frontBottom

Indicates that the light source is toward the bottom of the sensor.

case frontBottomLeft

Indicates that the light source is toward the bottom-left of the sensor.

case frontBottomRight

Indicates that the light source is toward the bottom-right of the sensor.

case frontLeft

Indicates that the light source is toward the left of the sensor.

case frontRight

Indicates that the light source is toward the right of the sensor.

case frontTop

Indicates that the light source is toward the top of the sensor.

case frontTopLeft

Indicates that the light source is toward the top-left of the sensor.

case frontTopRight

Indicates that the light source is toward the top-right of the sensor.

case unknown

Indicates that the sensor can’t determine the light source’s location.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Measuring light level

var chromaticity: SRAmbientLightSample.Chromaticity

A coordinate pair that describes the sample’s light brightness and tint.

struct Chromaticity

A coordinate pair that describes light brightness and tint.

var lux: Measurement&lt;UnitIlluminance>

An object that describes the sample’s luminous flux.

var placement: SRAmbientLightSample.SensorPlacement

The light’s location relative to the sensor.

