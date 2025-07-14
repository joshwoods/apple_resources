

- HealthKit
- HKError
- HKError.Code
-  HKError.Code.errorNoData 

Case

# HKError.Code.errorNoData

Data is unavailable for the requested query and predicate.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
case errorNoData
```

## Discussion

This error indicates that no data exists that corresponds to a particular query, so the system can’t calculate the query’s result. HKStatisticsQuery queries return this error when HealthKit can’t return the data needed to calculate the statistics.

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

case errorAnotherWorkoutSessionStarted

Another app started a workout session.

case errorUserExitedWorkoutSession

The user exited your application while a workout session was running.

