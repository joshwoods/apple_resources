

- Media Player
-  MPMediaPredicate 

Class

# MPMediaPredicate

An abstract class that defines classes for filtering media in a media query.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class MPMediaPredicate
```

## Overview

In media queries, a *predicate* is a statement of a logical condition that you want to test each media item against. The system returns the media items that satisfy the condition in the query result. Use this class’s concrete subclass, described in MPMediaPropertyPredicate, to define the filter in a media query to retrieve a subset of media items from the library. For more information about media queries, see MPMediaQuery.

## Relationships

### Inherits From

- NSObject

### Inherited By

- MPMediaPropertyPredicate

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

class MPMediaPropertyPredicate

A set of predicates for defining a filter in a media query.

