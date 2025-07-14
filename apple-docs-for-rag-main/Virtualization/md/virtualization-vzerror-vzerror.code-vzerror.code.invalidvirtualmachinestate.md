

- Virtualization
- VZError
- VZError.Code
-  VZError.Code.invalidVirtualMachineState 

Case

# VZError.Code.invalidVirtualMachineState

An invalid state error.

macOS 11.0+

``` source
case invalidVirtualMachineState
```

## Discussion

This error occurs when the virtual machine is in the wrong state for the current operation. For example, you might receive this error when you attempt to interact with a stopped or paused virtual machine.

## See Also

### Error codes

case internalError

An internal error, such as the VM unexpectedly stopping.

case invalidVirtualMachineConfiguration

An invalid configuration error.

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

