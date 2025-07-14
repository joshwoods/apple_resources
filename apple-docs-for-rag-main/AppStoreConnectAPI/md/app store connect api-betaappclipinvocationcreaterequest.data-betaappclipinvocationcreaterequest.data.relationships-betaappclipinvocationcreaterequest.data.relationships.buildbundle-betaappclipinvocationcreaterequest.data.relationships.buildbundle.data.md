

- App Store Connect API
- BetaAppClipInvocationCreateRequest
- 
  - BetaAppClipInvocationCreateRequest
- BetaAppClipInvocationCreateRequest.Data
- BetaAppClipInvocationCreateRequest.Data.Relationships
- BetaAppClipInvocationCreateRequest.Data.Relationships.BuildBundle
-  BetaAppClipInvocationCreateRequest.Data.Relationships.BuildBundle.Data 

Object

# BetaAppClipInvocationCreateRequest.Data.Relationships.BuildBundle.Data

The type and ID of the Build Bundles resource that you’re relating with the Beta App Clip Invocations resource you’re creating.

App Store Connect API 1.6+

``` source
object BetaAppClipInvocationCreateRequest.Data.Relationships.BuildBundle.Data
```

## Properties

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the related Build Bundles resource.

`type`

`string`

 (Required) 

The resource type.

Value: `buildBundles`

