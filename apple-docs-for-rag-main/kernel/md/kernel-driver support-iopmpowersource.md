

- Kernel
- Driver Support
-  IOPMPowerSource 

Class

# IOPMPowerSource

macOS 10.0+

``` source
class IOPMPowerSource : IOService
```

## Overview

See IOKit/pwr_mgt/IOPM.h for power source keys relevant to this class. These report-type keys are required for calls to IOPMPowerSource::setReportables(), and they define the IORegistry interface through which data is passed back up to the rest of the system.

A subclassing driver that doesn't want to do anything fancy should:

1.  Subclass IOPMPowerSource

2.  Install its own battery change notifications or polling routine that can converse with actual battery hardware.

3.  When battery state changes, change the relevant member variables through setCurrentCapacity() style accessors.

4.  Call updateStatus() on itself when all such settings have been updated.

The subclass driver should also initially populate its settings and call updateStatus() on launch.

Settings:

 ExternalConnected
 Type: bool
 IORegistry Key: kIOPMPSExternalConnectedKey
 True if computer is drawing external power

 ExternalChargeCapable
 Type: bool
 IORegistry Key: kIOPMPSExternalChargeCapableKey
 True if external power is capable of charging internal battery

 BatteryInstalled
 Type: bool
 IORegistry Key: kIOPMPSBatteryInstalledKey
 True if a battery is present; false if removed

 IsCharging
 Type: bool
 IORegistry Key: kIOPMPSIsChargingKey
 True if battery is charging itself from external power

 AtWarnLevel
 Type: bool
 IORegistry Key: kIOPMPSAtWarnLevelKey
 True if draining battery capacity and past warn level

 AtCriticalLevel
 Type: bool
 IORegistry Key: kIOPMPSAtCriticalLevelKey
 True if draining battery capacity and past critical level

 CurrentCapacity
 MaxCapacity
 Type: unsigned int
 IORegistry Key: kIOPMPSCurrentCapacityKey, kIOPMPSMaxCapacityKey
 Capacity measured in mAh

 TimeRemaining
 Type: int
 IORegistry Key: kIOPMPSTimeRemainingKey
 Time remaining measured in minutes

 Amperage
 Type: int
 IORegistry Key: kIOPMPSAmperageKey
 Current is measured in mA

 Voltage
 Type: unsigned int
 IORegistry Key: kIOPMPSVoltageKey
 Voltage measured in mV

 CycleCount
 Type: unsigned int
 IORegistry Key: kIOPMPSCycleCountKey
 Number of charge/discharge cycles

 AdapterInfo
 Type: int
 IORegistry Key: kIOPMPSAdapterInfoKey
 Power adapter information

 Location
 Type: int
 IORegistry Key: kIOPMPSLocationKey
 Clue about battery&#39;s location in machine - Left vs. Right

 ErrorCondition
 Type: OSSymbol
 IORegistry Key: kIOPMPSErrorConditionKey
 String describing error state of battery

 Manufacturer
 Type: OSSymbol
 IORegistry Key: kIOPMPSManufacturerKey
 String describing battery manufacturer

 Manufactured Date
 Type: unsigned 16-bit bitfield
 IORegistry Key: kIOPMPSManufactureDateKey
 Date is published in a bitfield per the Smart Battery Data spec rev 1.1
 in section 5.1.26
   Bits 0...4 => day (value 1-31; 5 bits)
   Bits 5...8 => month (value 1-12; 4 bits)
   Bits 9...15 => years since 1980 (value 0-127; 7 bits)

 Model
 Type: OSSymbol
 IORegistry Key: kIOPMPSModelKey
 String describing model number

 Serial
 Type: OSSymbol
 IORegistry Key: kIOPMPSSerialKey
 String describing serial number or unique info
 The serial number published hear bears no correspondence to the Apple serial
 number printed on each battery. This is a manufacturer serial number with
 no correlation to the printed serial number.

 LegacyIOBatteryInfo
 Type: OSDictionary
 IORegistry Key: kIOPMPSLegacyBatteryInfoKey
 Dictionary conforming to the OS X 10.0-10.4

## Topics

### Miscellaneous

powerSource

Creates a new IOPMPowerSource nub. Must be attached to IORegistry, and registered by provider.

setPSProperty

updateStatus

Must be called by physical battery controller when battery state has changed significantly.

### Instance Variables

settingsChangedSinceUpdate

properties

### Instance Methods

- adapterInfo

- amperage

- atCriticalLevel

- atWarnLevel

- batteryInstalled

- capacityPercentRemaining

- currentCapacity

- cycleCount

- errorCondition

- externalChargeCapable

- externalConnected

- free

- getMetaClass

- getPSProperty

- init

- isCharging

- legacyIOBatteryInfo

- location

- manufacturer

- maxCapacity

- model

- serial

- setAdapterInfo

- setAmperage

- setAtCriticalLevel

- setAtWarnLevel

- setBatteryInstalled

- setCurrentCapacity

- setCycleCount

- setErrorCondition

- setExternalChargeCapable

- setExternalConnected

- setIsCharging

- setLegacyIOBatteryInfo

- setLocation

- setManufacturer

- setMaxCapacity

- setModel

- setPSProperty

- setSerial

- setTimeRemaining

- setVoltage

- timeRemaining

- updateStatus

- voltage

### Type Methods

+ powerSource

## Relationships

### Inherits From

- IOService

## See Also

### Power Management

IOACPIPlatformDevice

IOACPIPlatformExpert

IOPMPowerSourceList

IOPMrootDomain

IOPowerConnection

IOPwrController

IOACPIAddress

IOACPIAddressSpaceDescriptor

IOACPIAddressSpaceHandler

IOACPIAddressSpaceID

IOPMPowerState

acknowledgeSleepWakeNotification

gIOACPIAddressKey

gIOACPIDeviceStatusKey

gIOACPIHardwareIDKey

gIOACPIPlane

gIOACPIUniqueIDKey

