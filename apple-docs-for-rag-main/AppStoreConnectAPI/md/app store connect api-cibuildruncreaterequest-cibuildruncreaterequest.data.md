

- App Store Connect API
- CiBuildRunCreateRequest
-  CiBuildRunCreateRequest.Data 

Object

# CiBuildRunCreateRequest.Data

The data element of the request you use to start a new Xcode Cloud build.

App Store Connect API 1.5+

``` source
object CiBuildRunCreateRequest.Data
```

## Properties

`attributes`

CiBuildRunCreateRequest.Data.Attributes

The attributes that describe the request that creates a Build Runs resource.

`relationships`

CiBuildRunCreateRequest.Data.Relationships

The types and IDs of the related data to update.

`type`

`string`

 (Required) 

The resource type.

Value: `ciBuildRuns`

## Topics

### Objects

object CiBuildRunCreateRequest.Data.Attributes

The attributes you set that describe the new Build Runs resource.

object CiBuildRunCreateRequest.Data.Relationships

The relationships to other resources that you can set with this request.

