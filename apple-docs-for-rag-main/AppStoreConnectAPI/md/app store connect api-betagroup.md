

- App Store Connect API
-  BetaGroup 

Object

# BetaGroup

The data structure that represents a Beta Groups resource.

App Store Connect API 1.0+

``` source
object BetaGroup
```

## Properties

`attributes`

BetaGroup.Attributes

The resource’s attributes.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the resource.

`relationships`

BetaGroup.Relationships

Navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `betaGroups`

`links`

ResourceLinks

Navigational links that include the self-link.

## Topics

### Objects

object BetaGroup.Attributes

Attributes with values that describe a beta group update request.

object BetaGroup.Relationships

The relationships you included in the request and those on which you can operate.

## See Also

### Objects

object BetaGroupResponse

A response that contains a single Beta Groups resource.

object BetaGroupsWithoutIncludesResponse

A response body that contains a list of beta groups without any includes.

object BetaGroupCreateRequest

The request body you use to create a Beta Group.

object BetaGroupUpdateRequest

The request body you use to update a Beta Group.

object BetaGroupBuildsLinkagesRequest

A request body you use to add or remove builds from a beta group.

object BetaGroupBetaTestersLinkagesRequest

A request body you use to add or remove beta testers from a beta group.

object BetaGroupBetaTestersLinkagesResponse

A response body that contains a list of related resource IDs.

object BetaGroupBuildsLinkagesResponse

A response body that contains a list of related resource IDs.

object BetaPublicLinkUsagesV1MetricResponse

object BetaGroupsResponse

A response that contains a list of Beta Group resources.

