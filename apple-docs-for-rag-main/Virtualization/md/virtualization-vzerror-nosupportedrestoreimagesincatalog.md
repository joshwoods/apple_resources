

- Virtualization
- VZError
-  noSupportedRestoreImagesInCatalog 

Type Property

# noSupportedRestoreImagesInCatalog

The restore image catalog has no supported restore images.

macOS 13.0+

``` source
static var noSupportedRestoreImagesInCatalog: VZError.Code { get }
```

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

static var restoreImageCatalogLoadFailed: VZError.Code

The restore image catalog failed to load.

static var restoreImageLoadFailed: VZError.Code

The restore image failed to load.

