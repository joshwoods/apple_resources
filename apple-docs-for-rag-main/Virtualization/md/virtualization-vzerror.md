

- Virtualization
-  VZError 

Structure

# VZError

Errors that you might encounter when configuring or using a VM.

macOS 11.0+

``` source
struct VZError
```

## Overview

The domain for these errors is VZErrorDomain. When an error originates in a different component, the NSError object contains the domain of that component.

## Topics

### Getting the error codes

static var internalError: VZError.Code

An internal error occurred.

static var invalidVirtualMachineConfiguration: VZError.Code

An invalid configuration error.

static var invalidVirtualMachineState: VZError.Code

An invalid state error.

static var invalidVirtualMachineStateTransition: VZError.Code

An invalid state transition error.

static var invalidDiskImage: VZError.Code

An invalid disk-image error.

static var networkError: VZError.Code

A network error, such as a failed connection.

static var notSupported: VZError.Code

The operation isn’t supported.

static var outOfDiskSpace: VZError.Code

The host is out of disk space.

static var operationCancelled: VZError.Code

The user canceled the installation of Rosetta or the app canceled the installation of a guest OS.

static var installationFailed: VZError.Code

An error occurred during installation.

static var installationRequiresUpdate: VZError.Code

The framework canceled the installation because the host requires a software update in order to complete the installation.

static var invalidRestoreImage: VZError.Code

The restore image is invalid.

static var invalidRestoreImageCatalog: VZError.Code

The restore image catalog is invalid.

static var noSupportedRestoreImagesInCatalog: VZError.Code

The restore image catalog has no supported restore images.

static var restoreImageCatalogLoadFailed: VZError.Code

The restore image catalog failed to load.

static var restoreImageLoadFailed: VZError.Code

The restore image failed to load.

static var restore: VZError.Code

The VM failed to restore from the save file.

static var save: VZError.Code

The VM failed to save to the save file.

static var deviceAlreadyAttached: VZError.Code

The device already has an attachment to the VM.

static var deviceInitializationFailure: VZError.Code

A device initialization failure.

static var deviceNotFound: VZError.Code

The framework can’t find the device.

static var usbControllerNotFound: VZError.Code

The framework can’t find the controller.

enum Code

Errors you might encounter when configuring or using a virtual machine.

### Accessing the error information

static var virtualMachineLimitExceeded: VZError.Code

Returns an error code that indicates whether the system exceeded the limit on the number of running virtual machines.

### Type properties

static var networkBlockDeviceDisconnected: VZError.Code

Returns a value that indicates the connection state of the network block device.

static var networkBlockDeviceNegotiationFailed: VZError.Code

Returns a value that indicates whether the network block device negotiation failed.

### Type Properties

static var errorDomain: String

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Errors

let VZErrorDomain: String

The error domain for the Virtualization framework.

