

- Virtualization
- VZMacOSRestoreImage
-  operatingSystemVersion 

Instance Property

# operatingSystemVersion

The operating system version this restore image contains.

macOS 12.0+

``` source
var operatingSystemVersion: OperatingSystemVersion { get }
```

## See Also

### Getting Information About the Restore Image

var buildVersion: String

The build version this restore image contains.

var isSupported: Bool

A Boolean value that indicates whether the current host supports this restore image.

var mostFeaturefulSupportedConfiguration: VZMacOSConfigurationRequirements?

This object represents the most fully featured configuration that’s supported by both the current host and by this restore image.

var url: URL

The URL of this restore image.

