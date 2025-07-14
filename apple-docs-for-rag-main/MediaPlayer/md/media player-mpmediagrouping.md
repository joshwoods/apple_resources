

- Media Player
-  MPMediaGrouping 

Enumeration

# MPMediaGrouping

Keys used to configure a media query.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum MPMediaGrouping
```

## Overview

The following code snippet shows how to apply a grouping key:

- Swift
- Objective-C

```
let everything = MPMediaQuery()
everything.groupingType = MPMediaGrouping.album
let collections = [everything]
```

```
MPMediaQuery *everything = [[MPMediaQuery alloc] init];
[everything setGroupingType: MPMediaGroupingAlbum];
NSArray *collections = [everything collections];
```

After running these code lines, the `collections` array contains all the matched media items grouped and sorted according to album name.

To obtain a sorted list of songs, configure a media query with the `MPMediaGroupingTitle` key, or take advantage of the title key being the default for a media query. In either case, each obtained media item is, in effect, its own collection.

Collections sort according to the same rules used by iTunes on the desktop. This includes respecting the primary system language chosen by the user. The system ignores leading articles during sorting, including “A,” “An,” and “The” when using English, or “L’,” “La,” and “Le” when using French. If you need precise control over sorting, implement it in your application.

## Topics

### Media query keys

case title

Groups and sorts media item collections by title. For songs, for example, the title is the song name. This is the default grouping key.

case album

Groups and sorts media item collections by album, and sorts songs within an album by track order.

case artist

Groups and sorts media item collections by performing artist.

case albumArtist

Groups and sorts media item collections by album artist (the primary performing artist for an album as a whole).

case composer

Groups and sorts media item collections by composer.

case genre

Groups and sorts media item collections by musical or film genre.

case playlist

Groups and sorts media item collections by playlist.

case podcastTitle

Groups and sorts media item collections by podcast title.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

var itemSections: [MPMediaQuerySection]?

An array representing the section grouping of the query’s specified media items.

var collectionSections: [MPMediaQuerySection]?

An array representing the section grouping of the query’s specified media item collections.

