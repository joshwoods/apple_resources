

- Media Player
- MPMediaQuery
-  artists() 

Type Method

# artists()

Creates a media query that matches music items and that groups and sorts collections by artist name.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class func artists() -> MPMediaQuery
```

## Return Value

A media query that matches media items of type music and has a grouping type of MPMediaGrouping.artist.

## Discussion

A media item can have more than one media type; for example, an item could be of types “music” and “podcast.” An artists() query matches all music items, whether or not they’re also of other media types.

## See Also

### Creating media queries

class func albums() -> MPMediaQuery

Creates a media query that matches music items and that groups and sorts collections by album name.

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

