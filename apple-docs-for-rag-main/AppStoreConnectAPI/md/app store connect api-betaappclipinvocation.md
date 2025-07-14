

- App Store Connect API
-  BetaAppClipInvocation 

Object

# BetaAppClipInvocation

The data structure that represents a Beta App Clip Invocations resource.

App Store Connect API 1.6+

``` source
object BetaAppClipInvocation
```

## Properties

`attributes`

BetaAppClipInvocation.Attributes

The attributes that describe the Beta App Clip Invocations resource.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies a Beta App Clip Invocations resource.

`links`

ResourceLinks

Navigational links that include the self-link.

`relationships`

BetaAppClipInvocation.Relationships

The navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `betaAppClipInvocations`

## Topics

### Objects

object BetaAppClipInvocation.Attributes

The attributes that describe a Beta App Clip Invocations resource.

object BetaAppClipInvocation.Relationships

The relationships of the Beta App Clip Invocations resource you included in the request and those on which you can operate.

## See Also

### Objects

object BetaAppClipInvocationResponse

A response that contains a single Beta App Clip Invocations resource.

object BetaAppClipInvocationCreateRequest

The request body you use to create an App Clip invocation for testers.

object BetaAppClipInvocationUpdateRequest

The request body you use to update a Beta App Clip Invocation.

