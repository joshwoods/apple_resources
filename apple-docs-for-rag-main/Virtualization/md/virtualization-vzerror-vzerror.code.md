

- Virtualization
- VZError
-  VZError.Code 

Enumeration

# VZError.Code

Errors you might encounter when configuring or using a virtual machine.

macOS 11.0+

``` source
enum Code
```

## Overview

The domain for these errors is VZErrorDomain. When an error originates in a different component, the NSError object contains the domain of that component.

## Topics

### Error codes

case internalError

An internal error, such as the VM unexpectedly stopping.

case invalidVirtualMachineConfiguration

An invalid configuration error.

case invalidVirtualMachineState

An invalid state error.

case invalidVirtualMachineStateTransition

An invalid state transition error.

case invalidDiskImage

An invalid disk-image error.

case virtualMachineLimitExceeded

Unable to create an additional VM.

case networkError

A network error, such as a failed connection error, occurred.

case notSupported

The host computer or operating system isn’t supported.

case outOfDiskSpace

The host is out of disk space.

case operationCancelled

The code that indicates user canceled the installation of Rosetta or the app canceled the installation of a guest OS.

case installationFailed

An error occurred during installation.

case installationRequiresUpdate

The VM requires a software update in order to complete the installation.

case invalidRestoreImage

The restore image is invalid.

case invalidRestoreImageCatalog

The restore image catalog is invalid.

case noSupportedRestoreImagesInCatalog

The restore image catalog has no supported restore images.

case restoreImageCatalogLoadFailed

The restore image catalog failed to load.

case restoreImageLoadFailed

The restore image failed to load.

case networkBlockDeviceNegotiationFailed

The connection or the negotiation with the network block device server failed.

case networkBlockDeviceDisconnected

The network block device client disconnected from the server.

case restore

The VM failed to restore from save file.

case save

The VM failed to save to the save file.

case deviceAlreadyAttached

The device already has an attachment to the VM.

case deviceInitializationFailure

A device initialization failure.

case deviceNotFound

The framework can’t find the device.

case usbControllerNotFound

The framework can’t find the controller.

case internalError

An internal error, such as the VM unexpectedly stopping.

case invalidVirtualMachineConfiguration

An invalid configuration error.

case invalidVirtualMachineState

An invalid state error.

case invalidVirtualMachineStateTransition

An invalid state transition error.

case invalidDiskImage

An invalid disk-image error.

case virtualMachineLimitExceeded

Unable to create an additional VM.

case networkError

A network error, such as a failed connection error, occurred.

case notSupported

The host computer or operating system isn’t supported.

case outOfDiskSpace

The host is out of disk space.

case operationCancelled

The code that indicates user canceled the installation of Rosetta or the app canceled the installation of a guest OS.

case installationFailed

An error occurred during installation.

case installationRequiresUpdate

The VM requires a software update in order to complete the installation.

case invalidRestoreImage

The restore image is invalid.

case invalidRestoreImageCatalog

The restore image catalog is invalid.

case noSupportedRestoreImagesInCatalog

The restore image catalog has no supported restore images.

case restoreImageCatalogLoadFailed

The restore image catalog failed to load.

case restoreImageLoadFailed

The restore image failed to load.

case networkBlockDeviceNegotiationFailed

The connection or the negotiation with the network block device server failed.

case networkBlockDeviceDisconnected

The network block device client disconnected from the server.

case restore

The VM failed to restore from save file.

case save

The VM failed to save to the save file.

case deviceAlreadyAttached

The device already has an attachment to the VM.

case deviceInitializationFailure

A device initialization failure.

case deviceNotFound

The framework can’t find the device.

case usbControllerNotFound

The framework can’t find the controller.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

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

