

- Apple Music API
- StationGenres
- StationGenres.Relationships
-  StationGenres.Relationships.StationGenresStationsRelationship 

Object

# StationGenres.Relationships.StationGenresStationsRelationship

A relationship from the station genre to associated stations.

Apple Music 1.0+

``` source
object StationGenres.Relationships.StationGenresStationsRelationship
```

## Properties

`href`

`string`

A relative location for the relationship.

`next`

`string`

A relative cursor to fetch the next paginated collection of resources in the relationship if more exist.

`data`

`[`Stations`]`

 (Required) 

Stations associated with the station genre.

