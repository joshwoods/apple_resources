

- Media Player
-  MPMediaQuery 

Class

# MPMediaQuery

A query that specifies a set of media items from the device’s media library using a filter and a grouping type.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class MPMediaQuery
```

## Mentioned in 

Playing audio using the built-in music player

## Overview

Filter and grouping types are both optional; an unqualified query matches the entire library.

A query has at most one grouping type. A query’s filter can consist of any number of media property predicates. You build filters using MPMediaPropertyPredicate objects, based on property keys described in MPMediaItem.

After creating and configuring a query, you use it to retrieve media items or media item collections. You can also use a query to retrieve an array of MPMediaQuerySection instances, useful for displaying the results of a query in the user interface of your app. See the itemSections and collectionSections properties.

This class includes several convenience constructors that each apply a grouping type and, in most cases, match a subset of the library. The following table summarizes the features of these constructors. See MPMediaItem for descriptions of the entries in the Filter column. See MPMediaGrouping for descriptions of the entries in the Grouping type column.

| Constructor name | Matches entire library | Filter | Grouping type |
|----|----|----|----|
| albums() | \- | music | MPMediaGrouping.album |
| artists() | \- | music | MPMediaGrouping.artist |
| audiobooks() | \- | audioBook | MPMediaGrouping.title |
| compilations() | \- | any with MPMediaItemPropertyIsCompilation | MPMediaGrouping.album |
| composers() | Yes | any | MPMediaGrouping.composer |
| genres() | Yes | any | MPMediaGrouping.genre |
| playlists() | Yes | any | MPMediaGrouping.playlist |
| podcasts() | \- | podcast | MPMediaGrouping.podcastTitle |
| songs() | \- | music | MPMediaGrouping.title |

## Topics

### Creating media queries

The class methods in this section create queries which you can use directly or modify as described in Configuring media queries.

## Discussion

For each class method, the system sets the query’s groupingType property automatically according to the name of the method. For example, the albums() method assigns a grouping type of MPMediaGrouping.album. The grouping type specifies the nature of the media item collections you can then retrieve from the query. Some class methods match the entire Music library while others match a subset, as described in the Discussion sections for each method.

class func albums() -> MPMediaQuery

Creates a media query that matches music items and that groups and sorts collections by album name.

class func artists() -> MPMediaQuery

Creates a media query that matches music items and that groups and sorts collections by artist name.

class func songs() -> MPMediaQuery

Creates a media query that matches music items and that groups and sorts collections by song name.

class func playlists() -> MPMediaQuery

Creates a media query that matches the entire library and that groups and sorts collections by playlist name.

class func podcasts() -> MPMediaQuery

Creates a media query that matches podcast items and that groups and sorts collections by podcast name.

class func audiobooks() -> MPMediaQuery

Creates a media query that matches audio book items and that groups and sorts collections by audio book name.

class func compilations() -> MPMediaQuery

Creates a media query that matches compilation items and that groups and sorts collections by album name.

class func composers() -> MPMediaQuery

Creates a media query that matches all media items and that groups and sorts collections by composer name.

class func genres() -> MPMediaQuery

Creates a media query that matches all media items and that groups and sorts collections by genre name.

init(filterPredicates: Set&lt;MPMediaPredicate>?)

Initializes a media query with a set of media property predicates.

### Configuring media queries

var filterPredicates: Set&lt;MPMediaPredicate>?

The media property predicates of the media query.

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

### Performing media queries

You obtain a specified array of media items or media item collections from the iPod library by calling the items or collections accessor methods.

var items: [MPMediaItem]?

An array of media items that match the media query’s predicate.

var collections: [MPMediaItemCollection]?

An array of media item collections whose contained items match the query’s media property predicate.

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

class MPMediaQuerySection

A range of media items or media item collections from within a media query.

class MPMediaPropertyPredicate

A set of predicates for defining a filter in a media query.

class MPMediaPredicate

An abstract class that defines classes for filtering media in a media query.

