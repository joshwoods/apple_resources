

- Roster API
-  Locations 

Object

# Locations

A list of locations, with a token for pagination.

Roster API 1.0.0+

``` source
object Locations
```

## Properties

`locations`

`[`Location`]`

A list of Location objects.

`moreToFollow`

`boolean`

A flag that indicates whether there are more locations. If `true`, use the `nextPageToken` to request another list from the remaining locations.

`nextPageToken`

`string`

A token to request additional locations, if any. Use this as the `nextPageToken` parameter for the List locations request.

## See Also

### Information about locations

Read a location

Returns a specific location in an Apple School Manager organization.

object Location

A location in an Apple School Manager organization.

List locations

Returns a list of locations in an Apple School Manager organization.

