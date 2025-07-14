

- FamilyControls
- FamilyControlsError
-  FamilyControlsError.restricted 

Case

# FamilyControlsError.restricted

A restriction prevents your app from using Family Controls on this device.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 13.0+

``` source
case restricted
```

## See Also

### Error Values

case invalidAccountType

The device isn’t signed into a valid iCloud account.

case authorizationConflict

Another authorized app already provides parental controls.

case authorizationCanceled

The parent or guardian canceled a request for authorization.

case invalidArgument

The method’s arguments are invalid.

case unavailable

The system failed to set up the Family Control framework.

case networkError

The device must be connected to the network in order to enroll with parental controls.

case authenticationMethodUnavailable

The device must have a passcode set in order for an individual to enroll with parental controls.

