

- Core HID
- HIDUsage
-  HIDUsage.ScalesUsage 

Enumeration

# HIDUsage.ScalesUsage

macOS 15.0+

``` source
enum ScalesUsage
```

## Topics

### Enumeration Cases

case calibrationCount

case dataScaling

case dataWeight

case enforcedZeroReturn

case reZeroCount

case scaleAttributeReport

case scaleClass

case scaleClassGeneric

case scaleClassIIIEnglish

case scaleClassIIILEnglish

case scaleClassIIILMetric

case scaleClassIIIMetric

case scaleClassIIMetric

case scaleClassIMetric

case scaleClassIVEnglish

case scaleClassIVMetric

case scaleControlReport

case scaleDataReport

case scaleDevice

case scaleStatisticsReport

case scaleStatus

case scaleStatusFault

case scaleStatusInMotion

case scaleStatusOverWeightLimit

case scaleStatusReport

case scaleStatusRequiresCalibration

case scaleStatusRequiresRezeroing

case scaleStatusStableAtCenterOfZero

case scaleStatusUnderZero

case scaleStatusWeightStable

case scaleWeightLimitReport

case scales

case weightUnit

case weightUnitAvoirTon

case weightUnitCarats

case weightUnitGrains

case weightUnitGram

case weightUnitKilogram

case weightUnitMetricTon

case weightUnitMilligram

case weightUnitOunce

case weightUnitPennyweights

case weightUnitPound

case weightUnitTaels

case weightUnitTroyOunce

case zeroScale

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

