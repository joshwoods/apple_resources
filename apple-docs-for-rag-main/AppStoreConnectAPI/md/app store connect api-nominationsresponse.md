

- App Store Connect API
-  NominationsResponse 

Object

# NominationsResponse

A response that contains a list of featuring nominations.

App Store Connect API 3.6+

``` source
object NominationsResponse
```

## Properties

`data`

`[`Nomination`]`

 (Required) 

`included`

`[*]`

Possible types: App`, `Actor`, `AppEvent`, `Territory

`links`

PagedDocumentLinks

 (Required) 

`meta`

PagingInformation

## See Also

### Objects

object Nomination

The data structure that represents a nomination resource.

object NominationUpdateRequest

The request body you use to update a featuring nomination.

object NominationCreateRequest

The request body you use to create a featuring nomination.

object NominationResponse

A response that contains a single featuring nomination resource.

