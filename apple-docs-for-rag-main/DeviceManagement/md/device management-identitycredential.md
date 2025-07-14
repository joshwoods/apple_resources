

- Device Management
-  IdentityCredential 

Object

# IdentityCredential

The data for a PKCS \#12 password-protected identity.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object IdentityCredential
```

## Properties

`Identity`

`string`

 (Required) 

The PKCS \#12 identity data.

`Password`

`string`

 (Required) 

The password required to decrypt the PKCS \#12 identity data.

## See Also

### Credentials

object ACMECredential

An ACME identity that the device generates.

object SCEPCredential

An SCEP identity that the device generates.

object UserNameAndPasswordCredential

Data that describes a credential that represents a user name and password.

