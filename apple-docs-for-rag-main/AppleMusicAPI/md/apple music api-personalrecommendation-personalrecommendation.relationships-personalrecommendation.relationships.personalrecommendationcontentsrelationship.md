

- Apple Music API
- PersonalRecommendation
- PersonalRecommendation.Relationships
-  PersonalRecommendation.Relationships.PersonalRecommendationContentsRelationship 

Object

# PersonalRecommendation.Relationships.PersonalRecommendationContentsRelationship

A relationship from the recommendation to its recommended content.

Apple Music 1.0+

``` source
object PersonalRecommendation.Relationships.PersonalRecommendationContentsRelationship
```

## Properties

`href`

`string`

A relative location for the relationship.

`next`

`string`

A relative cursor to fetch the next paginated collection of resources in the relationship if more exist.

`data`

`[`Resource`]`

 (Required) 

A list of recommended candidates that are a mixture of albums and playlists.

