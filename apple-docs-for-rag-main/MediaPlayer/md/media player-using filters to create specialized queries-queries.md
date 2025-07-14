

- Media Player
-  Using filters to create specialized queries 

Article

# Using filters to create specialized queries

Add a filter set to a query before populating a music player queue.

## Overview

Creating a queue and adding it to a music player is a straightforward task. You populate the music player queue by creating a basic query and searching the user’s music library for items that match the query. However, you can create filters and add them at query creation to refine the player’s music queue. Filter for an album, artist, song, or any of a variety of other options. For a list of keys you can use as filters, see General media item property keys.

### Create one or more filters

You need to create a new filter for each item you want to filter on. For example, if you want to filter for a specific album and all songs that contain a certain word from that album, you need two separate filters.

```
let albumTitleFilter =
    MPMediaPropertyPredicate(value: "Album Title",
                             forProperty: MPMediaItemPropertyAlbumTitle,
                             comparisonType: .equalTo)

let songTitleFilter =
    MPMediaPropertyPredicate(value: "Song Title",
                             forProperty: MPMediaItemPropertyTitle,
                             comparisonType: .contains)
```

### Combine the filters into a filter set

Combine the filters into a filter set before you assign it to a query.

```
let filterSet = Set([albumTitleFilter, songTitleFilter])
```

### Create a query using the filter set

Create a new query using the newly created filter set, and set the music player’s queue.

```
let query = MPMediaQuery(filterPredicates: filterSet)
musicPlayer.setQueue(with: query)
```

## See Also

### Media item queries

class MPMediaQuery

A query that specifies a set of media items from the device’s media library using a filter and a grouping type.

class MPMediaQuerySection

A range of media items or media item collections from within a media query.

class MPMediaPropertyPredicate

A set of predicates for defining a filter in a media query.

class MPMediaPredicate

An abstract class that defines classes for filtering media in a media query.

