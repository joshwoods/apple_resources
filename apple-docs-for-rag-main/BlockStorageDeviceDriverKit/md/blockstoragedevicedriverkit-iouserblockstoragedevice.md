

- BlockStorageDeviceDriverKit
-  IOUserBlockStorageDevice 

Class

# IOUserBlockStorageDevice

A DriverKit provider object that manages communications with a block storage device.

DriverKit 21.0+

``` source
class IOUserBlockStorageDevice;
```

## Overview

Implement your driver by subclassing this class and overriding all C++ pure virtual methods.

### Specifying the Driver’s Personality Information

When you subclass `IOUserBlockStorageDevice`, update the IOKitPersonalities key of your driver extension’s `Info.plist` file with information to match your driver to the correct hardware. For this class, always include the keys and values in the following table:

| Key                      | Value                              |
|--------------------------|------------------------------------|
| IOClass                  | `IOUserBlockStorageDevice`         |
| IOUserClass              | The name of your custom dext class |
| CFBundleIdentifierKernel | `com.apple.iokit.IOStorageFamily`  |

## Topics

### Running the Service

Override these functions from the base DriverKit framework in your driver class.

init

Handles the basic initialization of the service.

Start

Starts the current service and associates it with the specified provider.

Stop

Stops the service associated with the specified provider.

free

Performs any final cleanup for the service.

### Reporting Device Metadata

GetVendorString

Gets a string that identifies the vendor in response to a call from the framework.

GetProductString

Gets a string that identifies the product in response to a call from the framework.

GetRevisionString

Gets a string that identifies the current revision in response to a call from the framework.

GetAdditionalInfoString

Gets a string that provides additional information in response to a call from the framework.

DeviceString

A type that represents a string of character data from the device.

GetDeviceParams

Gets device parameters in response to a call from the framework.

DeviceParams

A structure that represents hardware-specific properties of the block storage device.

### Reporting Device Capabilities

ReportEjectability

Returns a Boolean value that indicates whether the media is ejectable, in response to a call from the framework.

ReportRemovability

Returns a Boolean value that indicates whether the media is removable, in response to a call from the framework.

ReportWriteProtection

Returns a Boolean value that indicates whether the media is write protected, in response to a call from the framework.

### Accessing the Device

DoAsyncUnmap

Sends an asynchronous request to the dext to reclaim storage by unmapping.

BlockRange

A structure that represents a range of blocks.

DoAsyncSynchronize

Forces the hardware buffer to flush data blocks to the media.

DoAsyncEjectMedia

Ejects the media.

Complete

Indicates that the dext completed an asynchronous call.

DoAsyncReadWrite

Starts an asynchronous read or write operation.

IOUserStorageOptions

Options that affect the performance of read-write operations.

CompleteIO

Indicates that the dext completed an asynchronous read-write call.

### Instance Methods

DoAsyncUnmapPriv

RegisterDext

## Relationships

### Inherits From

- IOService

