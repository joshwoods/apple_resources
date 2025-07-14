

- Core HID
- HIDUsage
-  HIDUsage.DigitizersUsage 

Enumeration

# HIDUsage.DigitizersUsage

macOS 15.0+

``` source
enum DigitizersUsage
```

## Topics

### Enumeration Cases

case altitude

case armature

case articulatedArm

case azimuth

case barrelPressure

case barrelSwitch

case batteryStrength

case brush

case buttonPressThreshold

case buttonSwitch

case capacitiveHeatMapDigitizer

case capacitiveHeatMapFrameData

case capacitiveHeatMapProtocolVendorID

case capacitiveHeatMapProtocolVersion

case characterGesture

case characterGestureData

case characterGestureDataLength

case chiselMarker

case contactCount

case contactCountMaximum

case contactIdentifier

case coordinateMeasuringMachine

case dataValid

case deviceConfiguration

case deviceIdentifier

case deviceMode

case deviceSettings

case deviceSupportedProtocols

case digitizer

case digitizer3D

case digitizerDiagnostic

case digitizerError

case eraser

case errorChargeLow

case errorFullTransFeaturesUnavailable

case errorNormalStatus

case errorTransducersExceeded

case finger

case freeSpaceWand

case gestureCharacterEnable

case gestureCharacterEncoding

case gestureCharacterQuality

case height

case highlighter

case inRange

case ink

case invert

case latencyMode

case lightPen

case microsoftPenProtocol

case multiplePointDigitizer

case noPreference

case noPreferredColor

case noProtocol

case padType

case pen

case pencil

case preferredColor

case preferredColorIsLocked

case preferredLineStyle

case preferredLineStyleIsLocked

case preferredLineWidth

case preferredLineWidthIsLocked

case programChangeKeys

case puck

case quality

case reportRate

case scanTime

case secondaryBarrelSwitch

case secondaryTipSwitch

case stereoPlotter

case stylus

case supportedReportRates

case surfaceSwitch

case switchDisabled

case switchUnimplemented

case tabletFunctionKeys

case tabletPick

case tap

case tipPressure

case tipSwitch

case touch

case touchPad

case touchScreen

case touchValid

case transducerConnected

case transducerIndex

case transducerIndexSelector

case transducerProductId

case transducerSerialNumber

case transducerSerialNumberPart2

case transducerSoftwareInfo

case transducerSupportedProtocols

case transducerSwitches

case transducerVendorId

case twist

case untouch

case usiProtocol

case utf16BigEndianCharacterGestureEncoding

case utf16LittleEndianCharacterGestureEncoding

case utf32BigEndianCharacterGestureEncoding

case utf32LittleEndianCharacterGestureEncoding

case utf8CharacterGestureEncoding

case wacomAESProtocol

case whiteboard

case width

case xTilt

case yTilt

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

