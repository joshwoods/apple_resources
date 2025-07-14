

- Enterprise Program API
-  Profile 

Object

# Profile

The data structure that represents a Profiles resource.

``` source
object Profile
```

## Properties

`attributes`

Profile.Attributes

The resource’s attributes.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the resource

`relationships`

Profile.Relationships

Navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `profiles`

`links`

ResourceLinks

Navigational links that include the self-link.

## Attributes 

Possible types:

## Topics

### Objects

object Profile.Attributes

Attributes that describe a Profiles resource.

object Profile.Relationships

The relationships you included in the request and those on which you can operate.

## See Also

### Objects

object ProfileCreateRequest

The request body you use to create a Profile.

object ProfileResponse

A response that contains a single Profiles resource.

object ProfilesResponse

A response that contains a list of Profiles resources.

object ProfilesWithoutIncludesResponse

