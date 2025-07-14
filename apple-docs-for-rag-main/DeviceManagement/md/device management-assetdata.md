

- Device Management
-  AssetData 

Object

# AssetData

A reference to arbitrary data with a specific media type.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object AssetData
```

## Properties

`Authentication`

AssetDataAuthenticationObject

The server authentication details.

`Reference`

AssetDataReferenceObject

 (Required) 

The external reference.

## Topics

### Supporting Objects

object AssetDataAuthenticationObject

The server authentication details for an asset data.

object AssetDataReferenceObject

The external reference for an asset data.

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

object AssetCredentialUserNameAndPassword

A reference to data that describes a credential that represents a user name and password.

object AssetUserIdentity

The user-identity data.

