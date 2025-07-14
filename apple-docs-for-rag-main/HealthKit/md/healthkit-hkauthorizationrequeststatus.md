

- HealthKit
-  HKAuthorizationRequestStatus 

Enumeration

# HKAuthorizationRequestStatus

Values that indicate whether your app needs to request authorization from the user.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 5.0+

``` source
enum HKAuthorizationRequestStatus
```

## Topics

### Statuses

case unknown

The authorization request status could not be determined because an error occurred.

case shouldRequest

The application has not yet requested authorization for all the specified data types.

case unnecessary

The application has already requested authorization for all the specified data types.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing HealthKit

func authorizationStatus(for: HKObjectType) -> HKAuthorizationStatus

Returns the app’s authorization status for sharing the specified data type.

enum HKAuthorizationStatus

Constants indicating the authorization status for a particular data type.

func getRequestStatusForAuthorization(toShare: Set&lt;HKSampleType>, read: Set&lt;HKObjectType>, completion: (HKAuthorizationRequestStatus, (any Error)?) -> Void)

Indicates whether the system presents the user with a permission sheet if your app requests authorization for the provided types.

class func isHealthDataAvailable() -> Bool

Returns a Boolean value that indicates whether HealthKit is available on this device.

func supportsHealthRecords() -> Bool

Returns a Boolean value that indicates whether the current device supports clinical records.

func requestAuthorization(toShare: Set&lt;HKSampleType>?, read: Set&lt;HKObjectType>?, completion: (Bool, (any Error)?) -> Void)

Requests permission to save and read the specified data types.

func requestAuthorization(toShare: Set&lt;HKSampleType>, read: Set&lt;HKObjectType>) async throws

Asynchronously requests permission to save and read the specified data types.

func requestPerObjectReadAuthorization(for: HKObjectType, predicate: NSPredicate?, completion: (Bool, (any Error)?) -> Void)

Asynchronously requests permission to read a data type that requires per-object authorization (such as vision prescriptions).

func handleAuthorizationForExtension(completion: (Bool, (any Error)?) -> Void)

Requests permission to save and read the data types specified by an extension.

var authorizationViewControllerPresenter: UIViewController?

The view controller that presents HealthKit authorization sheets.

