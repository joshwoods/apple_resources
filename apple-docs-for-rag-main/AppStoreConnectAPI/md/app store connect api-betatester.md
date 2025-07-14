

- App Store Connect API
-  BetaTester 

Object

# BetaTester

The data structure that represents a Beta Testers resource.

App Store Connect API 1.0+

``` source
object BetaTester
```

## Properties

`attributes`

BetaTester.Attributes

The resource’s attributes.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the resource.

`relationships`

BetaTester.Relationships

Navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `betaTesters`

`links`

ResourceLinks

Navigational links that include the self-link.

## Topics

### Attributes and Relationships

object BetaTester.Attributes

Attributes that describe a beta tester resource.

type BetaInviteType

String that indicates how you offer a beta invitation.

type BetaTesterState

String that describes the state of a beta tester.

object BetaTester.Relationships

The relationships you included in the request and those on which you can operate.

## See Also

### Objects

object BetaTestersWithoutIncludesResponse

object BetaTesterAppsLinkagesRequest

A request body you use to remove an app from a beta tester.

object BetaTesterAppsLinkagesResponse

A response body that contains a list of related resource IDs.

object BetaTesterBetaGroupsLinkagesRequest

A request body you use to add or remove beta groups from a beta tester.

object BetaTesterBetaGroupsLinkagesResponse

A response body that contains a list of related resource IDs.

object BetaTesterBuildsLinkagesRequest

A request body you use to add or remove builds from a beta tester.

object BetaTesterBuildsLinkagesResponse

A response body that contains a list of related resource IDs.

object BetaTesterCreateRequest

The request body you use to create a BetaTester.

object BetaTesterResponse

A response that contains a single Beta Testers resource.

object BetaTestersResponse

A response that contains a list of Beta Tester resources.

object AppsBetaTesterUsagesV1MetricResponse

A response that contains one or more beta app tester metric resources.

object BetaTesterUsagesV1MetricResponse

A response that contains one or more beta tester usage metric resources.

