

- Core HID
- HIDUsage
-  HIDUsage.HapticsUsage 

Enumeration

# HIDUsage.HapticsUsage

macOS 15.0+

``` source
enum HapticsUsage
```

## Topics

### Enumeration Cases

case autoTrigger

case autoTriggerAssociatedControl

case durationList

case intensity

case manualTrigger

case repeatCount

case retriggerPeriod

case simpleHapticController

case waveformBrushContinuous

case waveformBuzzContinuous

case waveformChiselMarkerContinuous

case waveformClick

case waveformCutoffTime

case waveformEraserContinuous

case waveformError

case waveformHover

case waveformInkContinuous

case waveformList

case waveformMarkerContinuous

case waveformNone

case waveformPencilContinuous

case waveformPress

case waveformRelease

case waveformRumbleContinuous

case waveformSparkleContinuous

case waveformStop

case waveformSuccess

case waveformVendorID

case waveformVendorPage

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

