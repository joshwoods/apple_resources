

- Media Player
-  MPMediaQuerySection 

Class

# MPMediaQuerySection

A range of media items or media item collections from within a media query.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
class MPMediaQuerySection
```

## Overview

You can use sections when displaying a query’s items or collections in your app’s user interface. You obtain an array of media query sections by using the itemSections or collectionSections properties of a media query (an instance of the MPMediaQuery class). The property values of a media query section are read-only.

## Topics

### Working with media query sections

var title: String

The localized title of the media query section.

var range: NSRange

The range in the media query’s items or collections array that the media query section represents.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Media item queries

Using filters to create specialized queries

Add a filter set to a query before populating a music player queue.

class MPMediaQuery

A query that specifies a set of media items from the device’s media library using a filter and a grouping type.

class MPMediaPropertyPredicate

A set of predicates for defining a filter in a media query.

class MPMediaPredicate

An abstract class that defines classes for filtering media in a media query.

