

- Virtualization
- VZMacOSRestoreImage
-  isSupported 

Instance Property

# isSupported

A Boolean value that indicates whether the current host supports this restore image.

macOS 13.0+

``` source
var isSupported: Bool { get }
```

## See Also

### Getting Information About the Restore Image

var buildVersion: String

The build version this restore image contains.

var mostFeaturefulSupportedConfiguration: VZMacOSConfigurationRequirements?

This object represents the most fully featured configuration that’s supported by both the current host and by this restore image.

var operatingSystemVersion: OperatingSystemVersion

The operating system version this restore image contains.

var url: URL

The URL of this restore image.

