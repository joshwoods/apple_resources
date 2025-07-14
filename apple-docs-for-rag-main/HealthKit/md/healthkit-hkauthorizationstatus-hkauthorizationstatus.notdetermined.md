

- HealthKit
- HKAuthorizationStatus
-  HKAuthorizationStatus.notDetermined 

Case

# HKAuthorizationStatus.notDetermined

The user has not yet chosen to authorize access to the specified data type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
case notDetermined
```

## Discussion

Make sure your app requests proper authorization before calling any other HealthKit methods. For more information on setting up HealthKit, see `HealthKit`.

## See Also

### Constants

case sharingDenied

The user has explicitly denied your app permission to save data of the specified type.

case sharingAuthorized

The user has explicitly authorized your app to save data of the specified type.

