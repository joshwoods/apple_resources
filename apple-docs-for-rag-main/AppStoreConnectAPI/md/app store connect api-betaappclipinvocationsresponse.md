

- App Store Connect API
-  BetaAppClipInvocationsResponse 

Object

# BetaAppClipInvocationsResponse

A response that contains a list of Beta App Clip Invocations resources.

App Store Connect API 1.6+

``` source
object BetaAppClipInvocationsResponse
```

## Properties

`data`

`[`BetaAppClipInvocation`]`

 (Required) 

The resource data.

`included`

`[`BetaAppClipInvocationLocalization`]`

The requested relationship data.

`links`

PagedDocumentLinks

 (Required) 

Navigational links that include the self-link.

`meta`

PagingInformation

The paging information.

## See Also

### Objects

object BuildBundle

The data structure that represents Build Bundles resource.

object AppClipDomainStatus

The data structure that represents the App Clip Domain Statuses resource.

object BuildBundleFileSize

The data structure that represents a Build Bundle File Sizes resource.

object AppClipDomainStatusResponse

A response that contains a single App Clip Domain Statuses resource.

object BuildBundleFileSizesResponse

A response that contains a list of Build Bundle File Sizes resources.

