

- Core HID
- HIDUsage
-  HIDUsage.VESAVirtualControlsUsage 

Enumeration

# HIDUsage.VESAVirtualControlsUsage

macOS 15.0+

``` source
enum VESAVirtualControlsUsage
```

## Topics

### Enumeration Cases

case autoSizeCenter

case blueVideoBlackLevel

case blueVideoGain

case bottomCornerDistortionBalance

case bottomCornerDistortionControl

case brightness

case contrast

case degauss

case focus

case greenVideoBlackLevel

case greenVideoGain

case horizontalFrequency

case horizontalLinearity

case horizontalLinearityBalance

case horizontalMisconvergence

case horizontalMoiré

case horizontalPincushion

case horizontalPincushionBalance

case horizontalPosition

case horizontalSize

case inputLevelSelect

case inputSourceSelect

case onScreenDisplay

case parallelogramDistortionKeyBalance

case polarityHorizontalSynchronization

case polarityVerticalSynchronization

case redVideoBlackLevel

case redVideoGain

case screenOrientation

case settings

case stereoMode

case synchronizationType

case tiltRotation

case topCornerDistortionBalance

case topCornerDistortionControl

case trapezoidalDistortionKey

case verticalFrequency

case verticalLinearity

case verticalLinearityBalance

case verticalMisconvergence

case verticalMoiré

case verticalPincushion

case verticalPincushionBalance

case verticalPosition

case verticalSize

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

