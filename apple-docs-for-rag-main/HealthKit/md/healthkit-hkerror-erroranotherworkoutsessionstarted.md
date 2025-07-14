

- HealthKit
- HKError
-  errorAnotherWorkoutSessionStarted 

Type Property

# errorAnotherWorkoutSessionStarted

Another app started a workout session.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
static var errorAnotherWorkoutSessionStarted: HKError.Code { get }
```

## Discussion

This error occurs whenever a second workout session is started. Apple Watch only runs one workout session at a time. If the user begins a second workout session in a different app, the original session receives this error message and then ends. The second session then starts.

## See Also

### Accessing errors

enum Code

Error codes returned by HealthKit.

static var noError: HKError.Code

No error occurred.

static var errorHealthDataUnavailable: HKError.Code

The user accessed HealthKit on an unsupported device.

static var errorHealthDataRestricted: HKError.Code

A Mobile Device Management (MDM) profile restricts the use of HealthKit on this device.

static var errorInvalidArgument: HKError.Code

The app passed an invalid argument to the HealthKit API.

static var errorAuthorizationDenied: HKError.Code

The user hasn’t given the app permission to save data.

static var errorAuthorizationNotDetermined: HKError.Code

The app hasn’t yet asked the user for the authorization required to complete the task.

static var errorRequiredAuthorizationDenied: HKError.Code

The user hasn’t granted the application authorization to access all the required clinical record types.

static var errorDatabaseInaccessible: HKError.Code

The HealthKit data is unavailable because it’s protected and the device is locked.

static var errorUserCanceled: HKError.Code

The user canceled the operation.

static var errorUserExitedWorkoutSession: HKError.Code

The user exited your application while a workout session was running.

static var errorNoData: HKError.Code

Data is unavailable for the requested query and predicate.

