

- App Store Connect API
- CiBuildRunCreateRequest
- 
  - CiBuildRunCreateRequest
- CiBuildRunCreateRequest.Data
- CiBuildRunCreateRequest.Data.Relationships
- CiBuildRunCreateRequest.Data.Relationships.PullRequest
-  CiBuildRunCreateRequest.Data.Relationships.PullRequest.Data 

Object

# CiBuildRunCreateRequest.Data.Relationships.PullRequest.Data

The type and ID of the Pull Requests resource that you’re relating with the Build Runs resource you’re creating.

App Store Connect API 1.5+

``` source
object CiBuildRunCreateRequest.Data.Relationships.PullRequest.Data
```

## Properties

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the related Pull Requests resource.

`type`

`string`

 (Required) 

The resource type.

Value: `scmPullRequests`

