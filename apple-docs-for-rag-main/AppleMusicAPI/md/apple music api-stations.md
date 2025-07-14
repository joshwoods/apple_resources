

- Apple Music API
-  Stations 

Object

# Stations

A resource object that represents a station.

Apple Music 1.0+

``` source
object Stations
```

## Properties

`id`

`string`

 (Required) 

The identifier for the station.

`type`

`string`

 (Required) 

This value must always be `stations`.

Value: `stations`

`href`

`string`

 (Required) 

The relative location for the station resource.

`attributes`

Stations.Attributes

The attributes for the station.

`relationships`

Stations.Relationships

The relationships for the station.

## Topics

### Related Objects

object Stations.Attributes

The attributes for a station resource.

object Stations.Relationships

The name of the relationship you want to fetch for this resource.

## See Also

### Handling the Response

object StationsResponse

The response to a stations request.

object StationGenres

A resource object that represents a station genre.

object StationGenresResponse

The response to a specific station genres resource request.

