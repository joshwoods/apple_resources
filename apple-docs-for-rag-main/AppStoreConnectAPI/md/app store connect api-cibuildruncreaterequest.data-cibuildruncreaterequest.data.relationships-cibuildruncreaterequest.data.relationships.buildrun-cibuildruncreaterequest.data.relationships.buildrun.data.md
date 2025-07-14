

- App Store Connect API
- CiBuildRunCreateRequest
- 
  - CiBuildRunCreateRequest
- CiBuildRunCreateRequest.Data
- CiBuildRunCreateRequest.Data.Relationships
- CiBuildRunCreateRequest.Data.Relationships.BuildRun
-  CiBuildRunCreateRequest.Data.Relationships.BuildRun.Data 

Object

# CiBuildRunCreateRequest.Data.Relationships.BuildRun.Data

The type and ID of the Build Runs resource that you’re relating with the Build Runs resource you’re creating.

App Store Connect API 1.5+

``` source
object CiBuildRunCreateRequest.Data.Relationships.BuildRun.Data
```

## Properties

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the related Build Runs resource.

`type`

`string`

 (Required) 

The resource type.

Value: `ciBuildRuns`

