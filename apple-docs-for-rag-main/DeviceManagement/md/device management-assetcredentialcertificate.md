

- Device Management
-  AssetCredentialCertificate 

Object

# AssetCredentialCertificate

A reference to a PKCS \#1 or PEM encoded certificate.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object AssetCredentialCertificate
```

## Properties

`Authentication`

AssetCredentialCertificateAuthenticationObject

The server authentication details.

`Reference`

AssetCredentialCertificateReferenceObject

 (Required) 

The external reference. Ensure that the asset data uses a media type of `application/pkcs1` or `application/pem` to correctly identify the type of encoded certificate. If the asset data includes a `ContentType` sub-key, set it to the corresponding media type.

## Topics

### Supporting Objects

object AssetCredentialCertificateAuthenticationObject

The server authentication details for an asset-credential certificate.

object AssetCredentialCertificateReferenceObject

The external reference for an asset-credential certificate.

## See Also

### Assets

object AssetCredentialACME

A reference to an ACME identity.

object AssetCredentialIdentity

A reference to a PKCS \#12 password-protected identity.

object AssetCredentialSCEP

A reference to an SCEP identity.

object AssetCredentialUserNameAndPassword

A reference to data that describes a credential that represents a user name and password.

object AssetData

A reference to arbitrary data with a specific media type.

object AssetUserIdentity

The user-identity data.

