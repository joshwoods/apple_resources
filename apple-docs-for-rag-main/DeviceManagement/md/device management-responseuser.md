

- Device Management
-  ResponseUser 

Object

# ResponseUser

The user in the organization.

Device Assignment ServicesVPP License Management

``` source
object ResponseUser
```

## Properties

`clientUserId`

`string`

The unique identifier for a user in your organization.

`email`

`string`

The user’s email address.

`idHash`

`string`

The hash of the user’s unique store identifier. The `idHash` field is only present when the user has an associated Apple ID.

`inviteCode`

`string`

The invitation code that associates an Apple ID to a user.

`status`

`string`

The current status of the user in the organization.

Possible Values: `Registered, Associated, Retired, Deleted`

## Mentioned in 

Managing Users

## See Also

### Objects and Data Types

object Asset

A product in the store.

object ResponseAsset

The asset that the organization owns.

object Assignment

The asset assignment for a user or device.

object RequestUser

The requested user in the organization.

