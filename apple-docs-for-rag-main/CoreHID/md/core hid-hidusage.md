

- Core HID
-  HIDUsage 

Enumeration

# HIDUsage

A type to represent HID usage pages.

macOS 15.0+

``` source
enum HIDUsage
```

## Overview

A HID usage page combines with a HID usage to specify the intended functionality for the associated item. Associated items can be descriptors, devices, reports, report data, elements, etc..

Currently unsupported cases can be used as HIDUsage.generic(_:_:), but may be added as supported cases later.

For more details, see Human Interface Devices (HID) Specifications and Tools.

## Topics

### Operators

static func == (HIDUsage, HIDUsage) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case arcade(HIDUsage.ArcadeUsage?)

case auxiliaryDisplay(HIDUsage.AuxiliaryDisplayUsage?)

case barcodeScanner(HIDUsage.BarcodeScannerUsage?)

case batterySystem(HIDUsage.BatterySystemUsage?)

case brailleDisplay(HIDUsage.BrailleDisplayUsage?)

case button(UInt16?)

case cameraControl(HIDUsage.CameraControlUsage?)

case consumer(HIDUsage.ConsumerUsage?)

case digitizers(HIDUsage.DigitizersUsage?)

case eyeAndHeadTrackers(HIDUsage.EyeAndHeadTrackersUsage?)

case fidoAlliance(HIDUsage.FIDOAllianceUsage?)

case gameControls(HIDUsage.GameControlsUsage?)

case generic(UInt16, UInt16?)

case genericDesktop(HIDUsage.GenericDesktopUsage?)

case genericDeviceControls(HIDUsage.GenericDeviceControlsUsage?)

case haptics(HIDUsage.HapticsUsage?)

case keyboardOrKeypad(HIDUsage.KeyboardOrKeypadUsage?)

case led(HIDUsage.LEDUsage?)

case lightingAndIllumination(HIDUsage.LightingAndIlluminationUsage?)

case magneticStripeReader(HIDUsage.MagneticStripeReaderUsage?)

case medicalInstrument(HIDUsage.MedicalInstrumentUsage?)

case monitor(HIDUsage.MonitorUsage?)

case monitorEnumerated(UInt16?)

case ordinal(UInt16?)

case physicalInputDevice(HIDUsage.PhysicalInputDeviceUsage?)

case power(HIDUsage.PowerUsage?)

case scales(HIDUsage.ScalesUsage?)

case sensors(HIDUsage.SensorsUsage?)

case simulationControls(HIDUsage.SimulationControlsUsage?)

case soc(HIDUsage.SOCUsage?)

case sportControls(HIDUsage.SportControlsUsage?)

case telephonyDevice(HIDUsage.TelephonyDeviceUsage?)

case vesaVirtualControls(HIDUsage.VESAVirtualControlsUsage?)

case vrControls(HIDUsage.VRControlsUsage?)

### Initializers

init(page: UInt16, usage: UInt16?)

Creates a HID usage page from raw page and usage values.

### Instance Properties

var hashValue: Int

The hash value.

var page: UInt16

The usage page value.

var usage: UInt16?

The usage value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Enumerations

enum ArcadeUsage

enum AuxiliaryDisplayUsage

enum BarcodeScannerUsage

enum BatterySystemUsage

enum BrailleDisplayUsage

enum ButtonUsage

enum CameraControlUsage

enum ConsumerUsage

enum DigitizersUsage

enum EyeAndHeadTrackersUsage

enum FIDOAllianceUsage

enum GameControlsUsage

enum GenericDesktopUsage

enum GenericDeviceControlsUsage

enum HapticsUsage

enum KeyboardOrKeypadUsage

enum LEDUsage

enum LightingAndIlluminationUsage

enum MagneticStripeReaderUsage

enum MedicalInstrumentUsage

enum MonitorEnumeratedUsage

enum MonitorUsage

enum OrdinalUsage

enum PhysicalInputDeviceUsage

enum PowerUsage

enum SOCUsage

enum ScalesUsage

enum SensorsUsage

enum SimulationControlsUsage

enum SportControlsUsage

enum TelephonyDeviceUsage

enum VESAVirtualControlsUsage

enum VRControlsUsage

### Default Implementations

CustomStringConvertible Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Interaction

Communicating with human interface devices

Interact with and obtain data from devices such as keyboards and mice.

actor HIDDeviceClient

A client of a physical or virtual HID compatible peripheral.

struct HIDElement

A representation of an item from a report descriptor for a HID device.

struct HIDElementCollection

A collection of items from a report descriptor for a HID device.

struct Value

Data associated with a HID element.

protocol HIDElementUpdate

A base protocol for element update types.

enum HIDReportType

Types for HID reports.

struct HIDReportID

A type to represent the report IDs of HID reports.

enum HIDDeviceError

Errors that the framework can throw.

enum HIDDeviceTransport

Common transport types that transmit data to or from a HID device.

enum HIDDeviceLocalizationCode

The localization codes that some HID devices declare to specify conformance to a certain format or language.

