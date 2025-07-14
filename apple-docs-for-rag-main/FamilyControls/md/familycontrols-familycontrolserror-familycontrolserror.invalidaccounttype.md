

- FamilyControls
- FamilyControlsError
-  FamilyControlsError.invalidAccountType 

Case

# FamilyControlsError.invalidAccountType

The device isn’t signed into a valid iCloud account.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 13.0+

``` source
case invalidAccountType
```

## Discussion

To request or revoke authorization, the user must sign into iCloud from a child account that’s part of a Family Sharing group.

## See Also

### Error Values

case authorizationConflict

Another authorized app already provides parental controls.

case authorizationCanceled

The parent or guardian canceled a request for authorization.

case invalidArgument

The method’s arguments are invalid.

case unavailable

The system failed to set up the Family Control framework.

case restricted

A restriction prevents your app from using Family Controls on this device.

case networkError

The device must be connected to the network in order to enroll with parental controls.

case authenticationMethodUnavailable

The device must have a passcode set in order for an individual to enroll with parental controls.

