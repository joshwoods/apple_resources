

- Core HID
- HIDUsage
-  HIDUsage.EyeAndHeadTrackersUsage 

Enumeration

# HIDUsage.EyeAndHeadTrackersUsage

macOS 15.0+

``` source
enum EyeAndHeadTrackersUsage
```

## Topics

### Enumeration Cases

case calibratedScreenHeight

case calibratedScreenWidth

case capabilities

case configuration

case configurationStatus

case control

case deviceModeRequest

case displayManufacturerDate

case displayManufacturerID

case displayProductID

case displaySerialNumber

case eyeTracker

case gazePoint

case headDirectionPoint

case headPosition

case headTracker

case leftEyePosition

case maximumScreenPlaneHeight

case maximumScreenPlaneWidth

case maximumTrackingDistance

case minimumTrackingDistance

case optimumTrackingDistance

case positionX

case positionY

case positionZ

case rightEyePosition

case rotationAboutXAxis

case rotationAboutYAxis

case rotationAboutZAxis

case samplingFrequency

case sensorTimestamp

case status

case trackerQuality

case trackingData

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

