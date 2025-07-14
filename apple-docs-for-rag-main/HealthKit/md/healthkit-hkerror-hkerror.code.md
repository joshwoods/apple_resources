

- HealthKit
- HKError
-  HKError.Code 

Enumeration

# HKError.Code

Error codes returned by HealthKit.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
enum Code
```

## Mentioned in 

Executing Statistics Collection Queries

## Topics

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

case errorNoData

Data is unavailable for the requested query and predicate.

### Enumeration Cases

case errorBackgroundWorkoutSessionNotAllowed

case errorDataSizeExceeded

case errorNotPermissibleForGuestUserMode

The app attempted to write HealthKit data while in a Guest User session in visionOS.

case errorWorkoutActivityNotAllowed

case unknownError

### Initializers

init?(rawValue: Int)

### Type Properties

static var noError: HKError.Code

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Errors

struct HKError

An error returned from a HealthKit method.

let HKErrorDomain: String

The domain for all HealthKit errors.

