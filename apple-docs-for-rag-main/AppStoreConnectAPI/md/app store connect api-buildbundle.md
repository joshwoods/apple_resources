

- App Store Connect API
-  BuildBundle 

Object

# BuildBundle

The data structure that represents Build Bundles resource.

App Store Connect API 1.6+

``` source
object BuildBundle
```

## Properties

`attributes`

BuildBundle.Attributes

The attributes that describe the Build Bundles resource.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies a Build Bundles resource.

`links`

ResourceLinks

Navigational links that include the self-link.

`relationships`

BuildBundle.Relationships

The navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `buildBundles`

## Topics

### Objects

object BuildBundle.Attributes

The attributes that describe a Build Bundles resource.

object BuildBundle.Relationships

The relationships of the Build Bundles resource you included in the request and those on which you can operate.

## See Also

### Objects

object AppClipDomainStatus

The data structure that represents the App Clip Domain Statuses resource.

object BuildBundleFileSize

The data structure that represents a Build Bundle File Sizes resource.

object AppClipDomainStatusResponse

A response that contains a single App Clip Domain Statuses resource.

object BetaAppClipInvocationsResponse

A response that contains a list of Beta App Clip Invocations resources.

object BuildBundleFileSizesResponse

A response that contains a list of Build Bundle File Sizes resources.

