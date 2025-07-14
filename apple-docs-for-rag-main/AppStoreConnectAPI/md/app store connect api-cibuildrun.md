

- App Store Connect API
-  CiBuildRun 

Object

# CiBuildRun

The data structure that represents a Build Runs resource.

App Store Connect API 1.5+

``` source
object CiBuildRun
```

## Properties

`attributes`

CiBuildRun.Attributes

The attributes that describe the Build Runs resource.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies a Build Runs resource.

`links`

ResourceLinks

The navigational links that include the self-link.

`relationships`

CiBuildRun.Relationships

The navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `ciBuildRuns`

## Topics

### Objects

object CiBuildRun.Attributes

The attributes that describe a Build Runs resource.

object CiBuildRun.Relationships

The relationships of the Build Runs resource you included in the request and those on which you can operate.

## See Also

### Objects

object CiBuildRunCreateRequest

The request body you use to start a new Xcode Cloud build.

object CiBuildRunResponse

A response that contains a single Build Runs resource.

object CiBuildActionsResponse

A response that contains a list of Build Actions resources.

