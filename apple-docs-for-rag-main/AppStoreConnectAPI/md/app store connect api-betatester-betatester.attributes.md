

- App Store Connect API
- BetaTester
-  BetaTester.Attributes 

Object

# BetaTester.Attributes

Attributes that describe a beta tester resource.

App Store Connect API 1.0+

``` source
object BetaTester.Attributes
```

## Properties

`email`

`email`

The beta tester’s email address, used for sending beta testing invitations.

`firstName`

`string`

The beta tester’s first name.

`inviteType`

BetaInviteType

An invite type that indicates if a beta tester was invited by an email invite or used a TestFlight public link to join a beta test.

`lastName`

`string`

The beta tester’s last name.

`state`

BetaTesterState

The status of a beta tester.

## Mentioned in 

App Store Connect API 3.5 release notes

## See Also

### Related Documentation

Beta Testers

People who can install and test prerelease builds.

### Attributes and Relationships

type BetaInviteType

String that indicates how you offer a beta invitation.

type BetaTesterState

String that describes the state of a beta tester.

object BetaTester.Relationships

The relationships you included in the request and those on which you can operate.

