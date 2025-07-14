

- HomeKit
- HMError
-  userIDNotEmailAddress 

Type Property

# userIDNotEmailAddress

An error indicating the user’s ID is not a valid email address.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
static var userIDNotEmailAddress: HMError.Code { get }
```

## See Also

### Detecting user errors

static var userDeclinedAddingUser: HMError.Code

An error indicating the user canceled the add user operation.

static var userDeclinedRemovingUser: HMError.Code

An error indicating the user canceled the remove user operation.

static var userDeclinedInvite: HMError.Code

An error indicating the user declined the invitation.

static var userManagementFailed: HMError.Code

A user management error not covered by the other errors.

