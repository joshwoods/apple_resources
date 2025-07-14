

- Apple Music API
-  StationGenres 

Object

# StationGenres

A resource object that represents a station genre.

Apple Music 1.0+

``` source
object StationGenres
```

## Properties

`id`

`string`

 (Required) 

The identifier for the station genre.

`type`

`string`

 (Required) 

This value must always be `station-genres`.

Value: `station-genres`

`href`

`string`

 (Required) 

The relative location for the station genre resource.

`attributes`

StationGenres.Attributes

The attributes for the station genre.

`relationships`

StationGenres.Relationships

The relationships for the station genre.

## Topics

### Related Objects

object StationGenres.Attributes

The attributes for the station genre resource.

object StationGenres.Relationships

The relationships for a station genre resource.

## See Also

### Handling the Response

object Stations

A resource object that represents a station.

object StationsResponse

The response to a stations request.

object StationGenresResponse

The response to a specific station genres resource request.

