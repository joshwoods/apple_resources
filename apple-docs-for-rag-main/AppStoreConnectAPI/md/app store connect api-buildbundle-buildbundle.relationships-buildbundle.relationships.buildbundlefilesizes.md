

- App Store Connect API
- BuildBundle
- BuildBundle.Relationships
-  BuildBundle.Relationships.BuildBundleFileSizes 

Object

# BuildBundle.Relationships.BuildBundleFileSizes

The data, links, and paging information that describe the relationship between the Build Bundles and the Build Bundle File Sizes resources.

App Store Connect API 1.6+

``` source
object BuildBundle.Relationships.BuildBundleFileSizes
```

## Properties

`data`

`[`BuildBundle.Relationships.BuildBundleFileSizes.Data`]`

The ID and type of the related Build Bundle File Sizes resource.

`links`

RelationshipLinks

Navigational links that include the self-link.

`meta`

PagingInformation

The paging information.

## Mentioned in 

App Store Connect API 1.6 release notes

## Topics

### Objects

object BuildBundle.Relationships.BuildBundleFileSizes.Data

The type and ID of a related Build Bundle File Sizes resource.

## See Also

### Objects

object BuildBundle.Relationships.AppClipDomainCacheStatus

The data and links that describe the relationship between the Build Bundles and the App Clip Domain Cache Statuses resources.

object BuildBundle.Relationships.AppClipDomainDebugStatus

The data and links that describe the relationship between the Build Bundles and the App Clip Domain Debug Statuses resources.

object BuildBundle.Relationships.BetaAppClipInvocations

The data, links, and paging information that describe the relationship between the Build Bundles and the Beta App Clip Invocations resources.

