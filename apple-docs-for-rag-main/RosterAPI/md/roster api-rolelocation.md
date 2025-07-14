

- Roster API
-  RoleLocation 

Object

# RoleLocation

A mapping between a role assumed by a user in an Apple School Manager organization, and the corresponding location.

Roster API 1.0.0+

``` source
object RoleLocation
```

## Properties

`locationId`

`string`

The identifier for the location where the User assumes the named role. This may identify a Location in the Apple School Manager organization, which you fetch with Read a location. Alternatively, it may identify the Organization, which you fetch with Read the organization.

`roleName`

`string`

The role the User assumes at the identified Location. Possible values for this property are `Student`, `Instructor`, and `Staff`.

## See Also

### Information about users

Read a user

Read a user in an Apple School Manager organization.

object User

A user in an Apple School Manager organization.

List users

List users in an Apple School Manager organization.

List users in a class

List users in a class of an Apple School Manager organization.

object Users

A list of users, with a token for pagination.

