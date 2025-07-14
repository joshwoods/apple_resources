

- Media Player
- MPMediaQuery
-  filterPredicates 

Instance Property

# filterPredicates

The media property predicates of the media query.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var filterPredicates: Set? { get set }
```

## Discussion

The General Media Item Property Keys and Podcast Item Property Keys enumerations in MPMediaItem contain the keys you can use to construct predicates.

## See Also

### Configuring media queries

func addFilterPredicate(MPMediaPredicate)

Adds a media property predicate to a query.

func removeFilterPredicate(MPMediaPredicate)

Removes a filter predicate from a query.

var groupingType: MPMediaGrouping

The grouping for collections retrieved with the media query.

var itemSections: [MPMediaQuerySection]?

An array representing the section grouping of the query’s specified media items.

var collectionSections: [MPMediaQuerySection]?

An array representing the section grouping of the query’s specified media item collections.

enum MPMediaGrouping

Keys used to configure a media query.

