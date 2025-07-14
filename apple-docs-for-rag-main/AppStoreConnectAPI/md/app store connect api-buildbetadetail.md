

- App Store Connect API
-  BuildBetaDetail 

Object

# BuildBetaDetail

The data structure that represents a Build Beta Details resource.

App Store Connect API 1.0+

``` source
object BuildBetaDetail
```

## Properties

`attributes`

BuildBetaDetail.Attributes

The resource’s attributes.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the resource.

`relationships`

BuildBetaDetail.Relationships

Navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `buildBetaDetails`

`links`

ResourceLinks

Navigational links that include the self-link.

## Topics

### Objects

object BuildBetaDetail.Attributes

Attributes that describe a Build Beta Details resource.

object BuildBetaDetail.Relationships

The relationships you included in the request and those on which you can operate.

## See Also

### Objects and Data Types

object BuildBetaDetailUpdateRequest

The request body you use to update a Build Data Detail.

object BuildBetaDetailResponse

A response that contains a single Build Beta Details resource.

object BuildBetaDetailsResponse

A response that contains a list of Build Beta Detail resources.

type ExternalBetaState

String that represents a build’s availability for external testing.

type InternalBetaState

String that represents a build’s availability for internal testing.

