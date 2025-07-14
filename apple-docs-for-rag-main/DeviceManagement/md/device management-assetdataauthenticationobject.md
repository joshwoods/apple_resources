

- Device Management
-  AssetDataAuthenticationObject 

Object

# AssetDataAuthenticationObject

The server authentication details for an asset data.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object AssetDataAuthenticationObject
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

object AssetDataReferenceObject

The external reference for an asset data.

