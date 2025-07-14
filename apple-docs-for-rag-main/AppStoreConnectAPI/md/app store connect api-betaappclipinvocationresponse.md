

- App Store Connect API
-  BetaAppClipInvocationResponse 

Object

# BetaAppClipInvocationResponse

A response that contains a single Beta App Clip Invocations resource.

App Store Connect API 1.6+

``` source
object BetaAppClipInvocationResponse
```

## Properties

`data`

BetaAppClipInvocation

 (Required) 

The resource data.

`included`

`[`BetaAppClipInvocationLocalization`]`

The requested relationship data.

`links`

DocumentLinks

 (Required) 

Navigational links that include the self-link.

## See Also

### Objects

object BetaAppClipInvocation

The data structure that represents a Beta App Clip Invocations resource.

object BetaAppClipInvocationCreateRequest

The request body you use to create an App Clip invocation for testers.

object BetaAppClipInvocationUpdateRequest

The request body you use to update a Beta App Clip Invocation.

