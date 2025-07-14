

- HealthKit
- HKError
- HKError.Code
-  HKError.Code.errorAuthorizationNotDetermined 

Case

# HKError.Code.errorAuthorizationNotDetermined

The app hasn’t yet asked the user for the authorization required to complete the task.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
case errorAuthorizationNotDetermined
```

## Mentioned in 

Authorizing access to health data

## Discussion

This error occurs when your app doesn’t request proper authorization before calling any other HealthKit methods. For more information on setting up HealthKit, see `HealthKit`.

## See Also

### Errors

case errorHealthDataUnavailable

HealthKit accessed on an unsupported device, such as an iPad.

case errorHealthDataRestricted

A Mobile Device Management (MDM) profile restricts the use of HealthKit on this device.

case errorInvalidArgument

The app passed an invalid argument to the HealthKit API.

case errorAuthorizationDenied

The user hasn’t given the app permission to save data.

case errorRequiredAuthorizationDenied

The user hasn’t granted the application authorization to access all the required clinical record types.

case errorDatabaseInaccessible

The HealthKit data is unavailable because it’s protected and the device is locked.

case errorUserCanceled

The user canceled the operation.

case errorAnotherWorkoutSessionStarted

Another app started a workout session.

case errorUserExitedWorkoutSession

The user exited your application while a workout session was running.

case errorNoData

Data is unavailable for the requested query and predicate.

