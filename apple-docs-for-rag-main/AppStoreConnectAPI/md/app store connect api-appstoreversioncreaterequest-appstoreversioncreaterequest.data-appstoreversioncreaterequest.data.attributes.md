

- App Store Connect API
- AppStoreVersionCreateRequest
- AppStoreVersionCreateRequest.Data
-  AppStoreVersionCreateRequest.Data.Attributes 

Object

# AppStoreVersionCreateRequest.Data.Attributes

Attributes that you set that describe the new resource.

App Store Connect API 1.2+

``` source
object AppStoreVersionCreateRequest.Data.Attributes
```

## Properties

`copyright`

`string`

`earliestReleaseDate`

`date-time`

`platform`

Platform

 (Required) 

`releaseType`

`string`

Possible Values: `MANUAL, AFTER_APPROVAL, SCHEDULED`

`reviewType`

`string`

Possible Values: `APP_STORE, NOTARIZATION`

`versionString`

`string`

 (Required) 

## See Also

### Objects

object AppStoreVersionCreateRequest.Data.Relationships

The relationships to other resources that you can set with this request.

