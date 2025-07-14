

- Virtualization
- VZMacOSRestoreImage
-  url 

Instance Property

# url

The URL of this restore image.

macOS 12.0+

``` source
var url: URL { get }
```

## Mentioned in 

Installing macOS on a Virtual Machine

## Discussion

If the restore image loaded using image(from:), the value of this property is a file URL.

If you obtain the restore image by fetching it from a server, use latestSupported and set the value of this property to a network URL for the installation media file.

## See Also

### Getting Information About the Restore Image

var buildVersion: String

The build version this restore image contains.

var isSupported: Bool

A Boolean value that indicates whether the current host supports this restore image.

var mostFeaturefulSupportedConfiguration: VZMacOSConfigurationRequirements?

This object represents the most fully featured configuration that’s supported by both the current host and by this restore image.

var operatingSystemVersion: OperatingSystemVersion

The operating system version this restore image contains.

