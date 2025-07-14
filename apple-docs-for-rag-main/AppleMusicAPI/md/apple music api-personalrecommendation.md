

- Apple Music API
-  PersonalRecommendation 

Object

# PersonalRecommendation

A resource object that represents recommended resources for a user calculated using their selected preferences.

Apple Music 1.0+

``` source
object PersonalRecommendation
```

## Properties

`id`

`string`

 (Required) 

The identifier for the recommendation.

`type`

`string`

 (Required) 

This value must always be `personal-recommendation`.

Value: `personal-recommendation`

`href`

`string`

 (Required) 

The relative location for the recommendation resource.

`attributes`

PersonalRecommendation.Attributes

The attributes for the recommendation.

`relationships`

PersonalRecommendation.Relationships

The relationships for the playlist.

## Topics

### Related Objects

object PersonalRecommendation.Attributes

The attributes for a recommendation resource.

object PersonalRecommendation.Relationships

The relationships for a recommendation resource.

## See Also

### Handling the Response

object PersonalRecommendationResponse

The response to a request for personal recommendations.

