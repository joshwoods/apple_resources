

- SensorKit
- SRElectrocardiogramData
-  SRElectrocardiogramData.Flags 

Structure

# SRElectrocardiogramData.Flags

Sensor context or events that occur during a sample ECG data reading.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
struct Flags
```

## Topics

### Getting context or events

static var crownTouched: SRElectrocardiogramData.Flags

The system records the ECG data when the person touches the crown.

static var signalInvalid: SRElectrocardiogramData.Flags

An invalid sensor signal occurs in the ECG data.

### Initializing flags

init(rawValue: UInt)

Initializes an ECG flags structure.

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

### Getting electrocardiogram details

var flags: SRElectrocardiogramData.Flags

var value: Measurement&lt;UnitElectricPotentialDifference>

The electrocardiogram data in microvolts.

