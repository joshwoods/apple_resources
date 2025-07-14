

- HealthKit
- HKError
- HKError.Code
-  HKError.Code.errorHealthDataUnavailable 

Case

# HKError.Code.errorHealthDataUnavailable

HealthKit accessed on an unsupported device, such as an iPad.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
case errorHealthDataUnavailable
```

## Discussion

Because iOS apps can run on devices that don’t support HealthKit (for example, on an iPad), always verify that the current device supports HealthKit by calling isHealthDataAvailable() before calling any other HealthKit methods. If HealthKit isn’t available on the device, other HealthKit methods fail with an errorHealthDataUnavailable error.

## See Also

### Errors

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

case errorAnotherWorkoutSessionStarted

Another app started a workout session.

case errorUserExitedWorkoutSession

The user exited your application while a workout session was running.

case errorNoData

Data is unavailable for the requested query and predicate.

