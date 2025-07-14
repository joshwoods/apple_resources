

- TVMLKit JS
- MediaItem
-  contentRatingRanking 

Instance Property

# contentRatingRanking

The rating for a video item.

tvOS 9.0+

``` source
attribute int contentRatingRanking;
```

## Discussion

The rating is a value from `0`-`1000`. This value corresponds to a specific rating used by different countries. For example, a rating value can represent a PG-13 rating in the United States and an MA15+ in Australia.

## See Also

### Rating Media Content

contentRatingDomain

The domain that the rating applies to.

isExplicit

A Boolean value indicating whether the item has explicit lyrics.

