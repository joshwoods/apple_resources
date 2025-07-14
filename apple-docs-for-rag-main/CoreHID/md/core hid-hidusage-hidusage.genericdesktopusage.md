

- Core HID
- HIDUsage
-  HIDUsage.GenericDesktopUsage 

Enumeration

# HIDUsage.GenericDesktopUsage

macOS 15.0+

``` source
enum GenericDesktopUsage
```

## Topics

### Enumeration Cases

case applicationBreak

case applicationDebuggerBreak

case assistiveControl

case byteCount

case callActiveLED

case callMuteLED

case callMuteToggle

case callStateManagementControl

case chassisEnclosure

case computerChassisDevice

case controlEnable

case coolantCriticalLevel

case coolantLevel

case coolantPump

case countedBuffer

case dPadDown

case dPadLeft

case dPadRight

case dPadUp

case deviceDock

case dial

case dockableDevice

case dockableDeviceDisplayOcclusion

case dockableDeviceDockingState

case dockableDeviceObjectType

case dockableDevicePrimaryUsageID

case dockableDevicePrimaryUsagePage

case dockableDeviceUniqueID

case dockableDeviceVendorID

case featureNotification

case gamepad

case hatSwitch

case indexTrigger

case joystick

case keyboard

case keypad

case motionWakeup

case mouse

case multiAxisController

case palmTrigger

case pointer

case portableDeviceControl

case qw

case qx

case qy

case qz

case resolutionMultiplier

case rpm

case rx

case ry

case rz

case select

case sensorZone

case slider

case spatialController

case start

case systemAppMenu

case systemBreak

case systemColdRestart

case systemContextMenu

case systemControl

case systemDebuggerBreak

case systemDismissNotification

case systemDisplayBoth

case systemDisplayDual

case systemDisplayExternal

case systemDisplayInternal

case systemDisplayInvert

case systemDisplayRotationLockButton

case systemDisplayRotationLockSliderSwitch

case systemDisplaySwapPrimaryOrSecondary

case systemDisplayToggleIntOrExtMode

case systemDisplayToggleLCDAutoscale

case systemDoNotDisturb

case systemDock

case systemFunctionShift

case systemFunctionShiftLock

case systemFunctionShiftLockIndicator

case systemHibernate

case systemMainMenu

case systemMenuDown

case systemMenuExit

case systemMenuHelp

case systemMenuLeft

case systemMenuRight

case systemMenuSelect

case systemMenuUp

case systemMicrophoneMute

case systemMultiAxisController

case systemPowerDown

case systemSetup

case systemSleep

case systemSpeakerMute

case systemUndock

case systemWakeUp

case systemWarmRestart

case tabletPCSystemControls

case thumbstick

case vbrx

case vbry

case vbrz

case vno

case vx

case vy

case vz

case waterCoolingDevice

case wheel

case wirelessRadioButton

case wirelessRadioControls

case wirelessRadioLED

case wirelessRadioSliderSwitch

case x

case y

case z

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

