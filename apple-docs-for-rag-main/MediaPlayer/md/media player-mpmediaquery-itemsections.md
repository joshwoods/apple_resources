

- Media Player
- MPMediaQuery
-  itemSections 

Instance Property

# itemSections

An array representing the section grouping of the query’s specified media items.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
var itemSections: [MPMediaQuerySection]? { get }
```

## Discussion

This property consists of an array of MPMediaQuerySection instances. The value of this property may be `nil` if there’s no appropriate section grouping of the media items.

## See Also

### Configuring media queries

var filterPredicates: Set&lt;MPMediaPredicate>?

The media property predicates of the media query.

func addFilterPredicate(MPMediaPredicate)

Adds a media property predicate to a query.

func removeFilterPredicate(MPMediaPredicate)

Removes a filter predicate from a query.

var groupingType: MPMediaGrouping

The grouping for collections retrieved with the media query.

var collectionSections: [MPMediaQuerySection]?

An array representing the section grouping of the query’s specified media item collections.

enum MPMediaGrouping

Keys used to configure a media query.

