

- HealthKit
- HKHealthStore
-  getRequestStatusForAuthorization(toShare:read:completion:) 

Instance Method

# getRequestStatusForAuthorization(toShare:read:completion:)

Indicates whether the system presents the user with a permission sheet if your app requests authorization for the provided types.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 5.0+

``` source
func getRequestStatusForAuthorization(
    toShare typesToShare: Set,
    read typesToRead: Set,
    completion: @escaping (HKAuthorizationRequestStatus, (any Error)?) -> Void
)
```

``` source
func statusForAuthorizationRequest(
    toShare typesToShare: Set,
    read typesToRead: Set
) async throws -> HKAuthorizationRequestStatus
```

## Discussion

When working with clinical types, users may need to reauthorize access when new data is added.

## See Also

### Accessing HealthKit

func authorizationStatus(for: HKObjectType) -> HKAuthorizationStatus

Returns the app’s authorization status for sharing the specified data type.

enum HKAuthorizationStatus

Constants indicating the authorization status for a particular data type.

enum HKAuthorizationRequestStatus

Values that indicate whether your app needs to request authorization from the user.

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

