

- App Store Connect API
-  ScmProvider 

Object

# ScmProvider

The data structure that represents a Providers resource.

App Store Connect API 1.5+

``` source
object ScmProvider
```

## Properties

`attributes`

ScmProvider.Attributes

The attributes that describe the Providers resource.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies a Providers resource.

`links`

ResourceLinks

The navigational links that include the self-link.

`relationships`

ScmProvider.Relationships

`type`

`string`

 (Required) 

The resource type.

Value: `scmProviders`

## Topics

### Objects and Types

object ScmProvider.Attributes

The attributes that describe a Providers resource.

object ScmProviderType

The source code management provider’s type.

### Dictionaries

object ScmProvider.Relationships

## See Also

### Objects

object ScmProviderResponse

A response that contains a single Providers resource.

object ScmProvidersResponse

A response that contains a list of Providers resources.

