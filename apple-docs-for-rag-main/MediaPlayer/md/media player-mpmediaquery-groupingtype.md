

- Media Player
- MPMediaQuery
-  groupingType 

Instance Property

# groupingType

The grouping for collections retrieved with the media query.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var groupingType: MPMediaGrouping { get set }
```

## Discussion

The default grouping type is MPMediaGrouping.title. See MPMediaGrouping for the list of available grouping types.

## See Also

### Configuring media queries

var filterPredicates: Set&lt;MPMediaPredicate>?

The media property predicates of the media query.

func addFilterPredicate(MPMediaPredicate)

Adds a media property predicate to a query.

func removeFilterPredicate(MPMediaPredicate)

Removes a filter predicate from a query.

var itemSections: [MPMediaQuerySection]?

An array representing the section grouping of the query’s specified media items.

var collectionSections: [MPMediaQuerySection]?

An array representing the section grouping of the query’s specified media item collections.

enum MPMediaGrouping

Keys used to configure a media query.

