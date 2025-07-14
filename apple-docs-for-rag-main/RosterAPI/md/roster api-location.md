

- Roster API
-  Location 

Object

# Location

A location in an Apple School Manager organization.

Roster API 1.0.0+

``` source
object Location
```

## Properties

`dateCreated`

`string`

The date the location object was created in Apple School Manager. The date string is in ISO 8601 format.

`dateLastModified`

`string`

The date the location object was modified in Apple School Manager. The date string is in ISO 8601 format.

`domain`

`string`

The location’s domain.

`id`

`string`

The location’s identifier.

`name`

`string`

The location’s name.

`timeZone`

`string`

The time zone used at the location.

## See Also

### Information about locations

Read a location

Returns a specific location in an Apple School Manager organization.

List locations

Returns a list of locations in an Apple School Manager organization.

object Locations

A list of locations, with a token for pagination.

