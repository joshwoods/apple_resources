

- Roster API
-  Classes 

Object

# Classes

A list of classes, with a token for pagination.

Roster API 1.0.0+

``` source
object Classes
```

## Properties

`classes`

`[`Class`]`

A list of Class objects.

`moreToFollow`

`boolean`

A flag that indicates whether there are more classes. If `true`, use the `nextPageToken` to request another list from the remaining classes.

`nextPageToken`

`string`

A token to request additional classes, if any. Use this as the `nextPageToken` parameter for the List classes request.

## See Also

### Information about classes

Read a class

Read a class from an Apple School Manager organization.

object Class

A class in an Apple School Manager organization.

List classes

List classes in an Apple School Manager organization.

