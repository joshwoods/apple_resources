

- DriverKit
-  IOService 

Class

# IOService

The base class for managing the setup and registration of your driver.

DriverKitiOSiPadOSmacOS

``` source
class IOService;
```

## Mentioned in 

Creating a Driver Using the DriverKit SDK

## Overview

An IOService object is the base class the system uses to represent all devices and device-related interfaces. When the user plugs in a device, the system creates one or more service objects to manage interactions with that device. One service object represents the device itself, and additional service objects represent the interfaces or communication protocols that the device supports. For example, the driver for a USB camera that supports multiple video and audio protocols might define different service objects for each protocol.

When the user plugs in a device, the system looks for the service objects that best match the device’s capabilities. Apple’s built-in driver families support most device types and a large array of standard interfaces. You provide custom service objects to support your device’s custom behaviors.

In most cases, you subclass a child of IOService such as IOUSBHostInterface, instead of IOService itself. Use the methods of this class to do the following:

- Handle the initialization, setup, and teardown of your driver.

- View and manage the I/O Registry entry for the device or interface.

- Configure the dispatch queue on which to execute your code.

- Respond to power-level changes

For additional information about how to implement services for a particular type of device, see the service subclasses in HIDDriverKit, USBDriverKit, NetworkingDriverKit, SerialDriverKit, and USBSerialDriverKit.

### Adding Member Variables to Your Custom Subclass

Don’t declare custom member variables directly in your IOService subclass. Instead, DriverKit requires you to define all variables in a separate structure. During initialization, allocate a block of memory for that structure and assign that block to the system-provided `ivars` variable of your service class. The following code example shows you how to define the structure and allocate it in the init method of your service class.

```
struct MyCustomKeyboardDriver_IVars
{
    OSArray *elements;

    struct {
        OSArray *elements;
    } keyboard;
};

bool MyCustomKeyboardDriver::init()
{
   if (!super::init()) {return false;}

   // Allocate memory for the instance variables.
   ivars = IONewZero(MyCustomKeyboardDriver_IVars, 1);
   if (!ivars) {return false;}

exit:
   return true;
}

```

Deallocate any memory that you allocate for your custom variables in the free method of your class.

## Topics

### Running the Service

init

Handles the basic initialization of the service.

Start

Starts the current service and associates it with the specified provider.

Stop

Stops the service associated with the specified provider.

free

Performs any final cleanup for the service.

### Registering the Service with IOKit

RegisterService

Starts the registration process for the service and performs any additional matching.

SetName

Sets the name of the service in the system’s registry.

GetRegistryEntryID

Returns the registry ID for the current service.

IOServiceName

A string type for setting the name of the service in the system’s registry.

### Managing the Registry Properties

CopyProperties

Returns the registry properties associated with the current service.

SetProperties

Sends the dictionary of properties to the current service object.

SearchProperty

Searches for a property with the specified name in the current service or one of its parent services, and returns the corresponding value.

IOPropertyName

A string type for specifying the name of a property in the system’s registry.

IORegistryPlaneName

A string type for specifying the name of a plane in the system’s registry.

Search Options

Options to apply when searching for registry properties.

### Configuring Additional Dispatch Queues

SetDispatchQueue

Associates a custom dispatch queue with the service and assigns the specified name to it.

CopyDispatchQueue

Gets the dispatch queue with the specified name from the current service.

### Responding to Power-Level Changes

SetPowerState

Updates the service in response to power-related changes for a provider.

ChangePowerState

Changes the device’s power state to the specified level.

Service Power Capabilities

Constants that indicate the power state of a device.

### Creating a New Service

NewUserClient

Requests the creation of a new user client for the service.

Create

Requests the creation of a new service object.

### Instance Methods

AdjustBusy

ClientCrashed

ConfigureReport

CopyName

CopyProviderProperties

CopySystemStateNotificationService

CoreAnalyticsSendEvent

CreateDefaultDispatchQueue

GetBusyState

GetProvider

JoinPMTree

RemoveProperty

RequireMaxBusStall

SetLegend

SetPowerOverride

StateNotificationItemCopy

StateNotificationItemCreate

StateNotificationItemSet

Stop_async

StringFromReturn

Terminate

UpdateReport

### Type Methods

CreateKernelClassMatchingDictionary

CreateKernelClassMatchingDictionary

CreateNameMatchingDictionary

CreateNameMatchingDictionary

CreatePropertyMatchingDictionary

CreatePropertyMatchingDictionary

CreateUserClassMatchingDictionary

CreateUserClassMatchingDictionary

## Relationships

### Inherits From

- OSObject

### Inherited By

- IOUserClient
- IOUserServer

## See Also

### Services

Creating a Driver Using the DriverKit SDK

Create a driver that supports proprietary features of your company’s hardware devices.

Debugging and testing system extensions

Debug your system extensions by temporarily disabling the security checks that macOS performs during the installation process.

