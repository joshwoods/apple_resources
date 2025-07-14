

- Device Management
-  AssetCredentialUserNameAndPasswordAuthenticationObject 

Object

# AssetCredentialUserNameAndPasswordAuthenticationObject

The server authentication details for an asset-credential user name and password.

iOS 15.0+iPadOS 15.0+macOS 13.0+tvOS 16.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object AssetCredentialUserNameAndPasswordAuthenticationObject
```

## Properties

`Type`

`string`

 (Required) 

The type of authentication, which has these allowed values:

- `MDM`: A request that uses MDM semantics, which includes the device-identity certificate and any user authentication. This is equivalent to an MDM request made to the `CheckInURL` or `ServerURL`. This option is only available through declarative device management.

- `None`: A standard GET request.

Possible Values: `MDM, None`

## See Also

### Supporting Objects

object AssetCredentialUserNameAndPasswordReferenceObject

The external reference for an asset-credential user name and password.

