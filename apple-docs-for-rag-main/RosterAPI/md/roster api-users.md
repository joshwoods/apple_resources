

- Roster API
-  Users 

Object

# Users

A list of users, with a token for pagination.

Roster API 1.0.0+

``` source
object Users
```

## Properties

`moreToFollow`

`boolean`

A flag that indicates whether there are more users. If `true`, use the `nextPageToken` to request another list from the remaining users.

`nextPageToken`

`string`

A token to request additional users, if any. Use this as the `nextPageToken` parameter for the List users request.

`users`

`[`User`]`

A list of User objects.

## See Also

### Information about users

Read a user

Read a user in an Apple School Manager organization.

object User

A user in an Apple School Manager organization.

object RoleLocation

A mapping between a role assumed by a user in an Apple School Manager organization, and the corresponding location.

List users

List users in an Apple School Manager organization.

List users in a class

List users in a class of an Apple School Manager organization.

