

- HealthKit
- HKHealthStore
-  isHealthDataAvailable() 

Type Method

# isHealthDataAvailable()

Returns a Boolean value that indicates whether HealthKit is available on this device.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
class func isHealthDataAvailable() -> Bool
```

## Return Value

true if HealthKit is available; otherwise, false.

## Mentioned in 

Authorizing access to health data

About the HealthKit framework

## Discussion

By default, HealthKit data is available on iOS, watchOS, and visionOS. HealthKit data is also available to iPads running iPadOS 17 or later, and to iOS apps running on Vision Pro. Devices running in an enterprise environment may restrict access to HealthKit data.

The HealthKit framework is available on devices running iPadOS 16 and earlier and macOS 13 and later, but your app can’t read or write HealthKit data. Calls to isHealthDataAvailable() return false.

## See Also

### Accessing HealthKit

func authorizationStatus(for: HKObjectType) -> HKAuthorizationStatus

Returns the app’s authorization status for sharing the specified data type.

enum HKAuthorizationStatus

Constants indicating the authorization status for a particular data type.

func getRequestStatusForAuthorization(toShare: Set&lt;HKSampleType>, read: Set&lt;HKObjectType>, completion: (HKAuthorizationRequestStatus, (any Error)?) -> Void)

Indicates whether the system presents the user with a permission sheet if your app requests authorization for the provided types.

enum HKAuthorizationRequestStatus

Values that indicate whether your app needs to request authorization from the user.

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

