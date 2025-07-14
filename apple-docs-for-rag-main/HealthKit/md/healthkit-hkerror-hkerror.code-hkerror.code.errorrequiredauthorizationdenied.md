

- HealthKit
- HKError
- HKError.Code
-  HKError.Code.errorRequiredAuthorizationDenied 

Case

# HKError.Code.errorRequiredAuthorizationDenied

The user hasn’t granted the application authorization to access all the required clinical record types.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 5.0+

``` source
case errorRequiredAuthorizationDenied
```

## Mentioned in 

Authorizing access to health data

## Discussion

You can specify required clinical record types using the NSHealthRequiredReadAuthorizationTypeIdentifiers `Info.plist` key.

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

