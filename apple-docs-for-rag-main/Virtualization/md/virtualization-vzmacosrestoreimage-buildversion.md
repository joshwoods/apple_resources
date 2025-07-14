

- Virtualization
- VZMacOSRestoreImage
-  buildVersion 

Instance Property

# buildVersion

The build version this restore image contains.

macOS 12.0+

``` source
var buildVersion: String { get }
```

## See Also

### Getting Information About the Restore Image

var isSupported: Bool

A Boolean value that indicates whether the current host supports this restore image.

var mostFeaturefulSupportedConfiguration: VZMacOSConfigurationRequirements?

This object represents the most fully featured configuration that’s supported by both the current host and by this restore image.

var operatingSystemVersion: OperatingSystemVersion

The operating system version this restore image contains.

var url: URL

The URL of this restore image.

