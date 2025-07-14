

- Device Management
-  AppManagedAppConfigDictionaryObject 

Object

# AppManagedAppConfigDictionaryObject

A dictionary of app config data and credentials.

iOS 18.4+iPadOS 18.4+visionOS 2.4+

``` source
object AppManagedAppConfigDictionaryObject
```

## Properties

`Certificates`

`[`AppManagedCredentialConfigObject`]`

Provides certificates to the managed app/extension. Each element in the array contains a certificate asset reference and an associated identifier, which the app/extension may use to look up the certificate.

`DataAssetReference`

`string`

Specifies the identifier of an asset declaration containing a reference to the app/extension config data. The corresponding asset must be of type `com.apple.asset.data`. The referenced data must be a property list file, and the asset’s “ContentType” value should be set to match the data type.

`Identities`

`[`AppManagedCredentialConfigObject`]`

Provides identities to the managed app/extension. Each element in the array contains an identity asset reference and an associated identifier, which the app/extension may use to look up the identity.

`Passwords`

`[`AppManagedCredentialConfigObject`]`

Provides passwords to the managed app/extension. Each element in the array contains a password asset reference and an associated identifier, which the app/extension may use to look up the password.

## See Also

### Objects

object AppManagedAttributesObject

A dictionary of values associated with an app.

object AppManagedCredentialConfigObject

A dictionary of values associated with a credential config.

object AppManagedExtensionConfigsObject

A dictionary of values associated with an extension config.

object AppManagedInstallBehaviorObject

A dictionary that describes how and when to install an app.

