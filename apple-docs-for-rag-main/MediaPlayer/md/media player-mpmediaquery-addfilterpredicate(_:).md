

- Media Player
- MPMediaQuery
-  addFilterPredicate(\_:) 

Instance Method

# addFilterPredicate(\_:)

Adds a media property predicate to a query.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func addFilterPredicate(_ predicate: MPMediaPredicate)
```

## Parameters 

`predicate`  

The media predicate to add to the set of predicates for the query.

## See Also

### Configuring media queries

var filterPredicates: Set&lt;MPMediaPredicate>?

The media property predicates of the media query.

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

