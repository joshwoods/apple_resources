

- Virtualization
- VZMacOSRestoreImage
-  mostFeaturefulSupportedConfiguration 

Instance Property

# mostFeaturefulSupportedConfiguration

This object represents the most fully featured configuration that’s supported by both the current host and by this restore image.

macOS 12.0+

``` source
@NSCopying
var mostFeaturefulSupportedConfiguration: VZMacOSConfigurationRequirements? { get }
```

## Mentioned in 

Installing macOS on a Virtual Machine

## See Also

### Getting Information About the Restore Image

var buildVersion: String

The build version this restore image contains.

var isSupported: Bool

A Boolean value that indicates whether the current host supports this restore image.

var operatingSystemVersion: OperatingSystemVersion

The operating system version this restore image contains.

var url: URL

The URL of this restore image.

