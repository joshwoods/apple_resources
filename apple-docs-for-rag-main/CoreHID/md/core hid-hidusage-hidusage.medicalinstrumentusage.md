

- Core HID
- HIDUsage
-  HIDUsage.MedicalInstrumentUsage 

Enumeration

# HIDUsage.MedicalInstrumentUsage

macOS 15.0+

``` source
enum MedicalInstrumentUsage
```

## Topics

### Enumeration Cases

case cine

case clipStore

case colorDopplerAdjust

case colorDopplerModeSelect

case depth

case depthGainCompensation

case focus

case freezeOrThaw

case medicalUltrasound

case microphoneEnable

case motionModeAdjust

case motionModeSelect

case next

case print

case save

case softControlAdjust

case softControlSelect

case softStepPrimary

case softStepSecondary

case spectralDopplerAdjust

case spectralDopplerModeSelect

case transmitPower

case twoDModeAdjust

case twoDModeSelect

case update

case vcrOrAcquisition

case volume

case zoomAdjust

case zoomSelect

### Initializers

init?(rawValue: UInt16)

Creates a new instance with the specified raw value.

### Instance Properties

var rawValue: UInt16

The corresponding value of the raw type.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static let page: UInt16

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

