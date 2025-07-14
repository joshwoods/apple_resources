

- Device Management
- ActiveNSExtensionsResponse
-  ActiveNSExtensionsResponse.ExtensionsItem 

Device Management Command

# ActiveNSExtensionsResponse.ExtensionsItem

A dictionary that contains information about an extension.

macOS 10.13+Device Assignment ServicesVPP License Management

``` source
object ActiveNSExtensionsResponse.ExtensionsItem
```

## Properties

`ContainerDisplayName`

`string`

The display name of the container.

`ContainerIdentifier`

`string`

The identifier of the container.

`DisplayName`

`string`

 (Required) 

The extension’s display name.

`ExtensionPoint`

`string`

 (Required) 

The NSExtensionPointIdentifier for the extension.

`Identifier`

`string`

 (Required) 

The identifier of the extension.

`Path`

`string`

 (Required) 

The path to the extension.

`UserElection`

`string`

 (Required) 

The user-selected state of the extension, which a user sets in the Extensions preference pane in System Preferences.

Possible Values: `Default, Use, Ignore`

`Version`

`string`

 (Required) 

The version of the extension.

## See Also

### Commands

object ActiveNSExtensionsResponse.ErrorChainItem

A dictionary that describes an error chain item.

