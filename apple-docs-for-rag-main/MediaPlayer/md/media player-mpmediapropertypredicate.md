

- Media Player
-  MPMediaPropertyPredicate 

Class

# MPMediaPropertyPredicate

A set of predicates for defining a filter in a media query.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class MPMediaPropertyPredicate
```

## Overview

Use one or more `MPMediaPropertyPredicate` objects to define the filter in a media query to retrieve a subset of media items from the Music library. A predicate in this context is a statement of a logical condition that you want to test each media item against. The query retrieves the items that satisfy that condition.

You define Music library queries, and retrieve query results, using the MPMediaQuery class. MPMediaItem and MPMediaItemCollection describe the media items and media item collections that you can retrieve with a query.

## Topics

### Creating media property predicates

init(value: Any?, forProperty: String)

Creates a media property predicate with the default comparison type.

init(value: Any?, forProperty: String, comparisonType: MPMediaPredicateComparison)

Creates a media property predicate with a specified comparison type.

### Examining media property predicates

var property: String

The property that the media property predicate uses when you invoke a query.

var value: Any?

The value that the media property predicate matches against when you invoke a query.

var comparisonType: MPMediaPredicateComparison

The type of matching comparison that the media property predicate performs when you invoke a query.

### Supporting types

enum MPMediaPredicateComparison

Logical comparison types for media queries.

## Relationships

### Inherits From

- MPMediaPredicate

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Media item queries

Using filters to create specialized queries

Add a filter set to a query before populating a music player queue.

class MPMediaQuery

A query that specifies a set of media items from the device’s media library using a filter and a grouping type.

class MPMediaQuerySection

A range of media items or media item collections from within a media query.

class MPMediaPredicate

An abstract class that defines classes for filtering media in a media query.

