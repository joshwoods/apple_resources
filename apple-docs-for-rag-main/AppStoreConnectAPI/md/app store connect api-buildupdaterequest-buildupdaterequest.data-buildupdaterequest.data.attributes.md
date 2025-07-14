

- App Store Connect API
- BuildUpdateRequest
- BuildUpdateRequest.Data
-  BuildUpdateRequest.Data.Attributes 

Object

# BuildUpdateRequest.Data.Attributes

Attributes whose values you’re changing as part of the update request.

App Store Connect API 1.0+

``` source
object BuildUpdateRequest.Data.Attributes
```

## Properties

`expired`

`boolean`

A Boolean value that indicates if the build has expired. An expired build is unavailable for testing.

`usesNonExemptEncryption`

`boolean`

A Boolean value that indicates whether the build uses non-exempt encryption.

## See Also

### Objects

object BuildUpdateRequest.Data.Relationships

The data and links that describe the relationship between the resources.

