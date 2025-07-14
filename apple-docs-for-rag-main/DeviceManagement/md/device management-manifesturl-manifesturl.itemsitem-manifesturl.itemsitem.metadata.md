

- Device Management
- ManifestURL
- ManifestURL.ItemsItem
-  ManifestURL.ItemsItem.Metadata 

Object

# ManifestURL.ItemsItem.Metadata

iOS 7.0+iPadOS 7.0+macOS 10.9+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object ManifestURL.ItemsItem.Metadata
```

## Properties

`bundle-identifier`

`string`

 (Required) 

`bundle-version`

`string`

`kind`

`string`

 (Required) 

Value: `software`

`subtitle`

`string`

`title`

`string`

 (Required) 

`items`

`[`ManifestURL.ItemsItem.Metadata.MetadataItemsItem`]`

Deprecated 

`sizeInBytes`

`integer`

Deprecated 

## Topics

### Objects

object ManifestURL.ItemsItem.Metadata.MetadataItemsItem

## See Also

### Commands

object InstallEnterpriseApplicationCommand.Command.Configuration

A dictionary that contains the configuration to install an enterprise app.

object InstallEnterpriseApplicationCommand.Command.Manifest

A dictionary that contains a manifest.

object ManifestURL

The URL to the app manifest.

