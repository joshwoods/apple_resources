

- SensorKit
- SRAmbientLightSample
-  SRAmbientLightSample.Chromaticity 

Structure

# SRAmbientLightSample.Chromaticity

A coordinate pair that describes light brightness and tint.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
struct Chromaticity
```

## Overview

The SRAmbientLightSample class provides read-only access to an instance of this structure through its chromaticity property.

## Topics

### Creating a Chromaticity

init()

Creates a chromaticity instance.

init(x: Float32, y: Float32)

Creates a chromaticity instance from the argument coordinate pair.

### Setting chromaticity

var x: Float32

The chromaticity x-value.

var y: Float32

The chromaticity y-value.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Measuring light level

var chromaticity: SRAmbientLightSample.Chromaticity

A coordinate pair that describes the sample’s light brightness and tint.

var lux: Measurement&lt;UnitIlluminance>

An object that describes the sample’s luminous flux.

var placement: SRAmbientLightSample.SensorPlacement

The light’s location relative to the sensor.

enum SensorPlacement

Directional values that describe light-source location with respect to the sensor.

