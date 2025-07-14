

- App Store Connect API
-  CiBuildAction 

Object

# CiBuildAction

The data structure that represents a Build Actions resource.

App Store Connect API 1.5+

``` source
object CiBuildAction
```

## Properties

`attributes`

CiBuildAction.Attributes

The attributes that describe the Build Actions resource.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies a Build Actions resource.

`links`

ResourceLinks

The navigational links that include the self-link.

`relationships`

CiBuildAction.Relationships

The navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `ciBuildActions`

## Topics

### Objects

object CiBuildAction.Attributes

The attributes that describe a Build Actions resource.

object CiBuildAction.Relationships

The relationships of the Build Actions resource you included in the request and those on which you can operate.

## See Also

### Objects

object CiArtifactsResponse

A response that contains a list of Artifacts resources.

object CiBuildActionResponse

A response that contains a single Build Actions resource.

object CiIssuesResponse

A response that contains a list of Issues resources.

object CiTestResultsResponse

A response that contains a list of Test Results resources.

