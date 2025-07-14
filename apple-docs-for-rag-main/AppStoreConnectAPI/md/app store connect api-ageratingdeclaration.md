

- App Store Connect API
-  AgeRatingDeclaration 

Object

# AgeRatingDeclaration

The data structure that represents an Age Rating Declarations resource.

App Store Connect API 1.2+

``` source
object AgeRatingDeclaration
```

## Properties

`attributes`

AgeRatingDeclaration.Attributes

Attributes that describe this Age Rating Declarations resource.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the resource.

`links`

ResourceLinks

Navigational links that include the self-link.

`type`

`string`

 (Required) 

The resource type.

Value: `ageRatingDeclarations`

## Topics

### Objects

object AgeRatingDeclaration.Attributes

Attributes that describe an Age Rating Declarations resource.

## See Also

### Objects and Data Types

object AgeRatingDeclarationUpdateRequest

The request body you use to update an Age Rating Declaration.

object AgeRatingDeclarationResponse

A response that contains a single Age Rating Declarations resource.

type AppStoreAgeRating

String that represents the app’s age rating as it appears on the App Store for all platforms.

type BrazilAgeRating

String that represents the app’s age rating as it appears on the App Store in Brazil for all platforms.

type KidsAgeBand

String that represents a Made for Kids app’s age band.

