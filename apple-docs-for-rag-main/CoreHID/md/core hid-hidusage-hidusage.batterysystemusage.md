

- Core HID
- HIDUsage
-  HIDUsage.BatterySystemUsage 

Enumeration

# HIDUsage.BatterySystemUsage

macOS 15.0+

``` source
enum BatterySystemUsage
```

## Topics

### Enumeration Cases

case absoluteStateOfCharge

case acPresent

case alarmInhibited

case atRate

case atRateOK

case atRateTimeToEmpty

case atRateTimeToFull

case averageCurrent

case averageTimeToEmpty

case averageTimeToFull

case batteryInsertion

case batteryPackModelLevel

case batteryPresent

case batterySupported

case belowRemainingCapacityLimit

case broadcastToCharger

case capacityGranularity1

case capacityGranularity2

case capacityMode

case chargeController

case chargerConnection

case chargerSelectorSupport

case chargerSpec

case charging

case chargingIndicator

case conditioningFlag

case connectionToSMBus

case currentNotRegulated

case currentOutOfRange

case cycleCount

case designCapacity

case discharging

case enablePolling

case fullChargeCapacity

case fullyCharged

case fullyDischarged

case iDeviceChemistry

case iDeviceName

case iManufacturerName

case inhibitCharge

case internalChargeController

case ioemInformation

case level2

case level3

case manufactureDate

case manufacturerAccess

case manufacturerData

case masterMode

case maxError

case needReplacement

case okToUse

case optionalManufacturingFunction1

case optionalManufacturingFunction2

case optionalManufacturingFunction3

case optionalManufacturingFunction4

case optionalManufacturingFunction5

case outputConnection

case powerFail

case primaryBattery

case primaryBatterySupport

case rechargable

case relativeStateOfCharge

case remainingCapacity

case remainingCapacityLimit

case remainingTimeLimit

case remainingTimeLimitExpired

case resetToZero

case runTimeToEmpty

case selectorRevision

case serialNumber

case smartBatteryAlarmWarning

case smartBatteryBatteryMode

case smartBatteryBatteryStatus

case smartBatteryChargerMode

case smartBatteryChargerSpecInfo

case smartBatteryChargerStatus

case smartBatteryErrorCode

case smartBatterySelectorInfo

case smartBatterySelectorPresets

case smartBatterySelectorState

case specificationInfo

case terminateCharge

case terminateDischarge

case thermistorCold

case thermistorHot

case thermistorOverRange

case thermistorUnderRange

case useNext

case voltageNotRegulated

case voltageOutOfRange

case warningCapacityLimit

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

