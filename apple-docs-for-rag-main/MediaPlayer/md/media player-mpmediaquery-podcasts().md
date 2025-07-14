

- Media Player
- MPMediaQuery
-  podcasts() 

Type Method

# podcasts()

Creates a media query that matches podcast items and that groups and sorts collections by podcast name.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class func podcasts() -> MPMediaQuery
```

## Return Value

A media query that matches media items of type podcast and that has a grouping type of MPMediaGrouping.podcastTitle. This query only returns podcasts downloaded to the user’s library.

## Discussion

A media item can have more than one media type; for example, an item could be of types “music” and “podcast.” A podcasts() query matches all podcast items, whether or not they’re also of other media types.

## See Also

### Creating media queries

class func albums() -> MPMediaQuery

Creates a media query that matches music items and that groups and sorts collections by album name.

class func artists() -> MPMediaQuery

Creates a media query that matches music items and that groups and sorts collections by artist name.

class func songs() -> MPMediaQuery

Creates a media query that matches music items and that groups and sorts collections by song name.

class func playlists() -> MPMediaQuery

Creates a media query that matches the entire library and that groups and sorts collections by playlist name.

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

