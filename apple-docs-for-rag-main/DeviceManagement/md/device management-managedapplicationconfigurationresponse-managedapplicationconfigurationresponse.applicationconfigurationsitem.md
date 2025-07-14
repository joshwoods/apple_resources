

- Device Management
- ManagedApplicationConfigurationResponse
-  ManagedApplicationConfigurationResponse.ApplicationConfigurationsItem 

Device Management Command

# ManagedApplicationConfigurationResponse.ApplicationConfigurationsItem

A dictionary that contains a managed app’s configurations item.

iOS 7.0+iPadOS 7.0+macOS 10.15+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object ManagedApplicationConfigurationResponse.ApplicationConfigurationsItem
```

## Properties

`Configuration`

ManagedApplicationConfigurationResponse.ApplicationConfigurationsItem.Configuration

The app’s configurations.

`Identifier`

`string`

 (Required) 

The app’s bundle identifier.

Note

For a watchOS app, the identifier is the watch’s bundle identifier, which differs from the main bundle identifier for the iPhone to which the watch is paired.

## Topics

### Commands

object ManagedApplicationConfigurationResponse.ApplicationConfigurationsItem.Configuration

A dictionary that contains a managed app’s configuration items.

## See Also

### Commands

object ManagedApplicationConfigurationResponse.ErrorChainItem

A dictionary that describes an error chain item.

