

- Apple Music API
- PersonalRecommendation
-  PersonalRecommendation.Attributes 

Object

# PersonalRecommendation.Attributes

The attributes for a recommendation resource.

Apple Music 1.0+

``` source
object PersonalRecommendation.Attributes
```

## Properties

`isGroupRecommendation`

`boolean`

Deprecated   (Required) 

Whether the recommendation is of group type.

`kind`

`string`

 (Required) 

The type of recommendation. Possible values are:

`music-recommendations`  
A recommendation for music content.

`recently-played`  
A recommendation based on recently played content.

`unknown`  
A generic recommendation type.

Possible Values: `music-recommendations, recently-played, unknown`

`nextUpdateDate`

`string`

 (Required) 

The next date in UTC format for updating the recommendation.

`reason`

PersonalRecommendation.Attributes.Reason

The localized reason for the recommendation.

`resourceTypes`

`[string]`

 (Required) 

The resource types supported by the recommendation.

`title`

PersonalRecommendation.Attributes.Title

The localized title for the recommendation.

## Topics

### Attribute Objects

object PersonalRecommendation.Attributes.Reason

An object that represents the reason for a personal recommendation.

object PersonalRecommendation.Attributes.Title

An object that represents the title of a personal recommendation.

## See Also

### Related Objects

object PersonalRecommendation.Relationships

The relationships for a recommendation resource.

