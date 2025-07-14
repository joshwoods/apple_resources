

- HealthKit
- HKError
- HKError.Code
-  HKError.Code.errorAnotherWorkoutSessionStarted 

Case

# HKError.Code.errorAnotherWorkoutSessionStarted

Another app started a workout session.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
case errorAnotherWorkoutSessionStarted
```

## Discussion

This error occurs whenever a second workout session is started. Apple Watch only runs one workout session at a time. If the user begins a second workout session in a different app, the original session receives this error message and then ends. The second session then starts.

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

case errorAuthorizationNotDetermined

The app hasn’t yet asked the user for the authorization required to complete the task.

case errorRequiredAuthorizationDenied

The user hasn’t granted the application authorization to access all the required clinical record types.

case errorDatabaseInaccessible

The HealthKit data is unavailable because it’s protected and the device is locked.

case errorUserCanceled

The user canceled the operation.

case errorUserExitedWorkoutSession

The user exited your application while a workout session was running.

case errorNoData

Data is unavailable for the requested query and predicate.

