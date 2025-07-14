

- Apple Music API
- Activities
- Activities.Relationships
-  Activities.Relationships.ActivitiesPlaylistsRelationship 

Object

# Activities.Relationships.ActivitiesPlaylistsRelationship

A relationship between the activity and its playlists.

Apple Music 1.0+

``` source
object Activities.Relationships.ActivitiesPlaylistsRelationship
```

## Properties

`href`

`string`

A relative location for the relationship.

`next`

`string`

A relative cursor to fetch the next paginated collection of resources in the relationship if more exist.

`data`

`[`Playlists`]`

 (Required) 

The playlists associated with this activity.

