

- SensorKit
- SRWristTemperature
-  SRWristTemperature.Condition 

Structure

# SRWristTemperature.Condition

The user activities with the watch that can impact the temperature measurement.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
struct Condition
```

## Topics

### Conditions

static var offWrist: SRWristTemperature.Condition

The watch being off the wrist impacts the accuracy.

static var onCharger: SRWristTemperature.Condition

The watch being on the charger impacts the accuracy.

static var inMotion: SRWristTemperature.Condition

The watch being in motion impacts the accuracy.

### Creating conditions

init(rawValue: UInt)

Creates and returns a new structure with the specified value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Determining the accuracy

var condition: SRWristTemperature.Condition

The condition of the measurement that impacts its accuracy.

