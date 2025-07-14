

- Core HID
- HIDUsage
-  HIDUsage.PowerUsage 

Enumeration

# HIDUsage.PowerUsage

macOS 15.0+

``` source
enum PowerUsage
```

## Topics

### Enumeration Cases

case activePower

case apparentPower

case audibleAlarmControl

case awaitingPower

case badCount

case battery

case batteryId

case batterySystem

case batterySystemId

case boost

case buck

case changedStatus

case charger

case chargerId

case communicationLost

case configActivePower

case configApparentPower

case configCurrent

case configFrequency

case configHumidity

case configPercentLoad

case configTemperature

case configVoltage

case current

case delayBeforeReboot

case delayBeforeShutdown

case delayBeforeStartup

case flow

case flowId

case frequency

case frequencyOutOfRange

case gang

case gangId

case good

case highVoltageTransfer

case humidity

case iManufacturer

case iName

case iProduct

case iSerialNumber

case initialized

case input

case inputId

case internalFailure

case lowVoltageTransfer

case moduleReset

case outlet

case outletId

case outletSystem

case outletSystemId

case output

case outputId

case overCharged

case overTemperature

case overload

case percentLoad

case powerConverter

case powerConverterId

case powerSummary

case powerSummaryId

case powerSupply

case present

case presentStatus

case shutdownImminent

case shutdownRequested

case switchOffControl

case switchOnControl

case switchOnOrOff

case switchable

case temperature

case test

case tested

case toggleControl

case ups

case used

case voltagOutOfRange

case voltage

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

