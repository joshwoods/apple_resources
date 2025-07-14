

- Device Management
-  SafariExtensionSettingsManagedExtensionsObject 

Object

# SafariExtensionSettingsManagedExtensionsObject

The dictionary that defines the managed extension.

iOS 18.0+iPadOS 18.0+macOS 15.0+Device Assignment ServicesVPP License Management

``` source
object SafariExtensionSettingsManagedExtensionsObject
```

## Properties

`ANY`

SafariExtensionSettingsExtensionDictionaryObject

The composed identifier of the managed extension, or “\*” for all extensions. In order for the extension to be managed, its host app must be present on the device.

To generate this string use `codesign -dv `. The browser extension is located in the PlugIns folder inside the app bundle. The expected format is “Identifier (TeamIdentifier)”.

For extensions that aren’t also available on macOS the app developer needs to provide this information.

## See Also

### Supporting Objects

object SafariExtensionSettingsExtensionDictionaryObject

The dictionary that defines the settings for the managed extension.

