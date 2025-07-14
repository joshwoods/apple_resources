

- Device Management
-  AssetCredentialIdentityReferenceObject 

Object

# AssetCredentialIdentityReferenceObject

A dictionary that describes the external reference.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object AssetCredentialIdentityReferenceObject
```

## Properties

`ContentType`

`string`

The media type that describes the data, which needs to use a URL that starts with `https://`. If present, the system checks the actual media type of the downloaded data, and an error occurs if the values don’t match.

`DataURL`

`string`

 (Required) 

The URL to retrieve data, which needs to start with `https://`.

`Hash-SHA-256`

`string`

A SHA-256 hash of the data stored at the `DataURL`, which needs to use a URL that starts with `https://`. Don’t set this value if `Size` is `0`, and the client ignores it. However, if present, the system checks the actual hash of the downloaded data, and an error occurs if the values don’t match.

`Size`

`integer`

The size of the data, which needs to use a URL that starts with `https://`. Set the size to `0` if there’s no expectation of a response body. If present, the system checks the actual size of the downloaded data, and an error occurs if the values don’t match.

## Discussion

Ensure that the asset data:

- Is a JSON document that represents the `com.apple.credential.identity` credential type

- Uses a media type of `application/json`, and if it includes a `ContentType` sub-key, that sub-key media type is also `application/json`

## See Also

### Supporting Objects

object AssetCredentialIdentityAuthenticationObject

The server authentication details for an asset-credential identity.

