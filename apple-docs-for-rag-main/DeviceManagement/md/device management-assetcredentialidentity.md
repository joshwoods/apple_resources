

- Device Management
-  AssetCredentialIdentity 

Object

# AssetCredentialIdentity

A reference to a PKCS \#12 password-protected identity.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object AssetCredentialIdentity
```

## Properties

`Accessible`

`string`

The keychain accessibility that determines when the keychain item is available for use, which has these allowed values:

- `Default`: The most restrictive accessibility that still satisfies all uses of the asset by configurations that reference it.

- `AfterFirstUnlock`: The keychain item is only available after the first unlock of the device.

Default: `Default`

Possible Values: `Default, AfterFirstUnlock`

`Authentication`

AssetCredentialIdentityAuthenticationObject

The server authentication details.

`Reference`

AssetCredentialIdentityReferenceObject

 (Required) 

The external reference. Ensure that the asset data:

- Is a JSON document that represents the `com.apple.credential.identity` credential type

- Uses a media type of `application/json`, and if it includes a `ContentType` sub-key, that sub-key media type is also `application/json`

## Topics

### Supporting Objects

object AssetCredentialIdentityAuthenticationObject

The server authentication details for an asset-credential identity.

object AssetCredentialIdentityReferenceObject

A dictionary that describes the external reference.

## See Also

### Assets

object AssetCredentialACME

A reference to an ACME identity.

object AssetCredentialCertificate

A reference to a PKCS \#1 or PEM encoded certificate.

object AssetCredentialSCEP

A reference to an SCEP identity.

object AssetCredentialUserNameAndPassword

A reference to data that describes a credential that represents a user name and password.

object AssetData

A reference to arbitrary data with a specific media type.

object AssetUserIdentity

The user-identity data.

