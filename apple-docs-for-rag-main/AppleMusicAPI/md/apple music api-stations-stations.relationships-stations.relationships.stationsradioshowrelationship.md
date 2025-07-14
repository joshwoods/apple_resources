

- Apple Music API
- Stations
- Stations.Relationships
-  Stations.Relationships.StationsRadioShowRelationship 

Object

# Stations.Relationships.StationsRadioShowRelationship

For radio show episodes, this relationship is the Apple Curator that represents the radio show.

Apple Music 1.0+

``` source
object Stations.Relationships.StationsRadioShowRelationship
```

## Properties

`data`

`[`AppleCurators`]`

 (Required) 

A collection of resources in the relationship.

`href`

`string`

A relative location to fetch the relationship, if it may be fetched directly.

`next`

`string`

A relative cursor to fetch the next paginated collection of resources in the relationship if more exist.

