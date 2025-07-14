

- Core HID
- HIDUsage
-  HIDUsage.PhysicalInputDeviceUsage 

Enumeration

# HIDUsage.PhysicalInputDeviceUsage

macOS 15.0+

``` source
enum PhysicalInputDeviceUsage
```

## Topics

### Enumeration Cases

case actuatorOverrideSwitch

case actuatorPower

case actuatorsEnabled

case attackLevel

case attackTime

case axesEnable

case blockHandle

case blockLoadError

case blockLoadFull

case blockLoadSuccess

case blockType

case centerPointOffset

case createNewEffectParameterBlockReport

case customForceData

case customForceDataOffset

case customForceDataReport

case customForceVendorDefinedData

case dcContinue

case dcDisableActuators

case dcEnableActuators

case dcPause

case dcReset

case dcStopAllEffects

case deadBand

case deviceGain

case deviceGainReport

case deviceManagedPool

case devicePaused

case direction

case directionEnable

case downloadForceSample

case duration

case effectOperation

case effectOperationReport

case effectParameterBlockFreeReport

case effectParameterBlockIndex

case effectParameterBlockLoadReport

case effectParameterBlockLoadStatus

case effectPlaying

case effectType

case etConstantForce

case etCustomForce

case etDamper

case etFriction

case etInertia

case etRamp

case etSawtoothDown

case etSawtoothUp

case etSine

case etSpring

case etSquare

case etTriangle

case fadeLevel

case fadeTime

case gain

case isochCustomForceEnable

case loopCount

case magnitude

case moveDestination

case moveLength

case moveSource

case negativeCoefficient

case negativeSaturation

case normal

case offset

case opEffectStart

case opEffectStartSolo

case opEffectStop

case parameterBlockMoveReport

case parameterBlockOffset

case parameterBlockPoolsReport

case parameterBlockSize

case period

case phase

case physicalInputDevice

case pidDeviceControl

case pidDeviceControlReport

case pidStateReport

case poolAlignment

case positiveCoefficient

case positiveSaturation

case ramPoolAvailable

case ramPoolSize

case rampEnd

case rampStart

case romEffectBlockCount

case romFlag

case romPoolSize

case safetySwitch

case sampleCount

case samplePeriod

case setConditionReport

case setConstantForceReport

case setCustomForceReport

case setEffectReport

case setEnvelopeReport

case setPeriodicReport

case setRampForceReport

case sharedParameterBlocks

case simultaneousEffectsMax

case startDelay

case triggerButton

case triggerRepeatInterval

case typeSpecificBlockHandle

case typeSpecificBlockOffset

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

