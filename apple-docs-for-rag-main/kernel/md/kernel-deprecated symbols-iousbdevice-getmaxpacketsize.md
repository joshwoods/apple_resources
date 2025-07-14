

- Kernel
- Deprecated Symbols
- IOUSBDevice
-  GetMaxPacketSize 

# GetMaxPacketSize

``` source
virtual UInt8 GetMaxPacketSize(
 void); 
```

## Overview

returns the maximum packet size for endpoint zero (only 8, 16, 32, 64 are valid)

## See Also

### Miscellaneous

CreateInterfaceIterator

DeviceRequest(IOUSBDevRequest *, UInt32, UInt32, IOUSBCompletion *)

execute a control request to the default control pipe (pipe zero)

DeviceRequest(IOUSBDevRequestDesc *, UInt32, UInt32, IOUSBCompletion *)

execute a control request to the default control pipe (pipe zero)

DisplayUserNotification

Will use the Notification Center to display a notification to the user. Only Low Power and Overcurrent notifications are supported.

DoLocationOverrideAndModelMatch

Will look for a kOverrideIfAtLocationID array proerty with locationID entries and a "MacModel" property. If any of the locationIDs match to the Mac Model, will return true. If there is no kOverrideAtLocationID property, it will also return true.

FindNextInterface

FindNextInterfaceDescriptor

GetAddress

GetBus

GetBusPowerAvailable

GetChildLocationID

GetConfiguration

GetConfigurationDescriptor

GetDeviceInformation

Returns status information about the USB device, such as whether the device is captive or whether it is in the suspended state.

GetDeviceRelease

GetDeviceStatus

GetExtraPowerAllocated

Clients can use this API to ask how much extra power has already been reserved by this device. Units are milliAmps (mA).

GetFullConfigurationDescriptor

GetHubParent

Used by the hub driver to give the nub a pointer to its HubPolicyMaker object

GetManufacturerStringIndex

GetNumConfigurations

GetPipeZero

GetProductID

GetProductStringIndex

GetSerialNumberStringIndex

GetSpeed

GetStringDescriptor

GetVendorID

MakePipe

build a pipe on a given endpoint

OpenOrCloseAllInterfacePipes

Iterates over all interfaces and either opens all the pipes, or closes them all

ReEnumerateDevice

Instruct the hub to which this device is attached to reset the port to which this device is attached. This causes the IOUSBDevice object and any child objects (IOUSBInterface objects or driver objects) to be terminated, and the device to be completely reenumerated, as if it had been detached and reattached.

RequestExtraPower

Clients can use this API to reserve extra power for use by this device while the machine is asleep or while it is awake. Units are milliAmps (mA).

ResetDevice

ReturnExtraPower

Clients can use this API to tell the system that they will not use power that was previously reserved by using the RequestExtraPower API.

SetAddress

SetConfiguration(IOService *, UInt8, bool)

SetConfiguration(IOService *, UInt8, bool, bool)

SetHubParent

Used by the hub driver to give the nub a pointer to its HubPolicyMaker object

SuspendDevice

Instruct the hub to which this device is attached to suspend or resume the port to which the device is attached. Note that if there are any outstanding transactions on any pipes in the device, those transactions will get returned with a kIOReturnNotResponding error.

