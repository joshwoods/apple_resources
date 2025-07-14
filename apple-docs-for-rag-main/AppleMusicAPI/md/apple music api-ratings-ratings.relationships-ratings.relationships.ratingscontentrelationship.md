

- Apple Music API
- Ratings
- Ratings.Relationships
-  Ratings.Relationships.RatingsContentRelationship 

Object

# Ratings.Relationships.RatingsContentRelationship

A relationship between the rating and the assocaited content.

Apple Music 1.0+

``` source
object Ratings.Relationships.RatingsContentRelationship
```

## Properties

`data`

`[*]`

 (Required) 

The content associated with the rating.

Possible types: Albums`, `LibraryMusicVideos`, `LibraryPlaylists`, `LibrarySongs`, `MusicVideos`, `Playlists`, `Songs`, `Stations

`href`

`string`

A relative location for the relationship.

`next`

`string`

A relative cursor to fetch the next paginated collection of resources in the relationship if more exist.

