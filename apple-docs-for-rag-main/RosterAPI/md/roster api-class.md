

- Roster API
-  Class 

Object

# Class

A class in an Apple School Manager organization.

Roster API 1.0.0+

``` source
object Class
```

## Properties

`dateCreated`

`string`

The date the class object was created in Apple School Manager. The date string is in ISO 8601 format.

`dateLastModified`

`string`

The date the class object was modified in Apple School Manager. The date string is in ISO 8601 format.

`id`

`string`

A unique identifier for this class.

`instructorIds`

`[string]`

A list of user identifiers for instructers. Values refer to the `id` field of the User object.

`room`

`string`

The name of the room.

`studentIds`

`[string]`

A list of user identifiers for students in the class.

`name`

`string`

The name of the class.

`number`

`string`

The number of the class.

`displayName`

`string`

The Class Nickname in Apple School Manager.

`locationId`

`string`

An identifier for the class’s location.

## See Also

### Information about classes

Read a class

Read a class from an Apple School Manager organization.

List classes

List classes in an Apple School Manager organization.

object Classes

A list of classes, with a token for pagination.

