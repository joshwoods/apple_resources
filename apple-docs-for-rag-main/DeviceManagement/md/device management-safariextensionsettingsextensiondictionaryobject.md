

- Device Management
-  SafariExtensionSettingsExtensionDictionaryObject 

Object

# SafariExtensionSettingsExtensionDictionaryObject

The dictionary that defines the settings for the managed extension.

iOS 18.0+iPadOS 18.0+macOS 15.0+Device Assignment ServicesVPP License Management

``` source
object SafariExtensionSettingsExtensionDictionaryObject
```

## Properties

`AllowedDomains`

`[string]`

Controls the domains and sub-domains the extension is granted access to. Any non-prefixed domains take precedence over prefixed domains, and `DeniedDomains` takes precedence over `AllowedDomains`. Any domains not specified in `AllowedDomains` or `DeniedDomains` are configurable by the user.

`DeniedDomains`

`[string]`

Controls the domains and sub-domains the extension isn’t allowed to access. Any non-prefixed domains take precedence over prefixed domains, and `DeniedDomains` takes precedence over `AllowedDomains`. Any domains not specified in `AllowedDomains` or `DeniedDomains` are configurable by the user.

`PrivateBrowsing`

`string`

Controls whether an extension is allowed in Private Browsing.

- `Allowed` - The user is allowed to turn the extension on or off in Private Browsing.

- `AlwaysOn` - The extension will always be on in Private Browsing if the extension is on outside of Private Browsing.

- `AlwaysOff` - The extension will never be on in Private Browsing.

Possible Values: `Allowed, AlwaysOn, AlwaysOff`

`State`

`string`

Controls whether an extension is allowed.

- `Allowed` - The user is allowed to turn the extension on or off.

- `AlwaysOn` - The extension will always be on.

- `AlwaysOff` - The extension will always be off.

Possible Values: `Allowed, AlwaysOn, AlwaysOff`

## See Also

### Supporting Objects

object SafariExtensionSettingsManagedExtensionsObject

The dictionary that defines the managed extension.

