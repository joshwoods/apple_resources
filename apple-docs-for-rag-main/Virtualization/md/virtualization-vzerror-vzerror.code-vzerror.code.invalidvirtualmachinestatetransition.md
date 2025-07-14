

- Virtualization
- VZError
- VZError.Code
-  VZError.Code.invalidVirtualMachineStateTransition 

Case

# VZError.Code.invalidVirtualMachineStateTransition

An invalid state transition error.

macOS 11.0+

``` source
case invalidVirtualMachineStateTransition
```

## Discussion

This error occurs when you attempt to change the state of the virtual machine in an invalid way. For example, it occurs when you attempt to start a virtual machine when its canStart property is false.

## See Also

### Error codes

case internalError

An internal error, such as the VM unexpectedly stopping.

case invalidVirtualMachineConfiguration

An invalid configuration error.

case invalidVirtualMachineState

An invalid state error.

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

