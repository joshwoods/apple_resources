

- Media Player
- MPMediaQuery
-  composers() 

Type Method

# composers()

Creates a media query that matches all media items and that groups and sorts collections by composer name.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class func composers() -> MPMediaQuery
```

## Return Value

A media query that matches all media items and that has a grouping type of MPMediaGrouping.composer.

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

class func podcasts() -> MPMediaQuery

Creates a media query that matches podcast items and that groups and sorts collections by podcast name.

class func audiobooks() -> MPMediaQuery

Creates a media query that matches audio book items and that groups and sorts collections by audio book name.

class func compilations() -> MPMediaQuery

Creates a media query that matches compilation items and that groups and sorts collections by album name.

class func genres() -> MPMediaQuery

Creates a media query that matches all media items and that groups and sorts collections by genre name.

init(filterPredicates: Set&lt;MPMediaPredicate>?)

Initializes a media query with a set of media property predicates.

