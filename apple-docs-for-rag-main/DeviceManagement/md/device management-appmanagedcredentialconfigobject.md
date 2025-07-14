

- Device Management
-  AppManagedCredentialConfigObject 

Object

# AppManagedCredentialConfigObject

A dictionary of values associated with a credential config.

iOS 17.2+iPadOS 17.2+visionOS 2.4+Device Assignment ServicesVPP License Management

``` source
object AppManagedCredentialConfigObject
```

## Properties

`AssetReference`

`string`

 (Required) 

Specifies the identifier of an asset declaration containing a user name and password. The password is made available to the managed app/extension. The user name is ignored.

`Identifier`

`string`

 (Required) 

The app/extension uses this identifier to fetch the corresponding password using the ManagedApp framework. App developers will define what values can be used for these identifiers.

## See Also

### Objects

object AppManagedAppConfigDictionaryObject

A dictionary of app config data and credentials.

object AppManagedAttributesObject

A dictionary of values associated with an app.

object AppManagedExtensionConfigsObject

A dictionary of values associated with an extension config.

object AppManagedInstallBehaviorObject

A dictionary that describes how and when to install an app.

