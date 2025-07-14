

- Device Management
-  AssetCredentialUserNameAndPassword 

Object

# AssetCredentialUserNameAndPassword

A reference to data that describes a credential that represents a user name and password.

iOS 15.0+iPadOS 15.0+macOS 13.0+tvOS 16.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object AssetCredentialUserNameAndPassword
```

## Properties

`Authentication`

AssetCredentialUserNameAndPasswordAuthenticationObject

The server authentication details.

`Reference`

AssetCredentialUserNameAndPasswordReferenceObject

 (Required) 

The external reference. Ensure that the asset data:

- Is a JSON document that represents the `com.apple.credential.usernameandpassword` credential type

- Uses a media type of `application/json`, and if it includes a `ContentType` sub-key, that sub-key media type is also `application/json`

## Topics

### Supporting Objects

object AssetCredentialUserNameAndPasswordAuthenticationObject

The server authentication details for an asset-credential user name and password.

object AssetCredentialUserNameAndPasswordReferenceObject

The external reference for an asset-credential user name and password.

## See Also

### Assets

object AssetCredentialACME

A reference to an ACME identity.

object AssetCredentialCertificate

A reference to a PKCS \#1 or PEM encoded certificate.

object AssetCredentialIdentity

A reference to a PKCS \#12 password-protected identity.

object AssetCredentialSCEP

A reference to an SCEP identity.

object AssetData

A reference to arbitrary data with a specific media type.

object AssetUserIdentity

The user-identity data.

