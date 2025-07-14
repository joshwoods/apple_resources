

- HealthKit
- HKHealthStore
-  authorizationStatus(for:) 

Instance Method

# authorizationStatus(for:)

Returns the app’s authorization status for sharing the specified data type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
func authorizationStatus(for type: HKObjectType) -> HKAuthorizationStatus
```

## Parameters 

`type`  

The type of data. This can be any concrete subclass of the HKObjectType class (any of the HKCharacteristicType , HKQuantityType, HKCategoryType, HKWorkoutType or HKCorrelationType classes).

## Return Value

A value indicating the app’s authorization status for this type. For a list of possible values, see HKAuthorizationStatus.

## Mentioned in 

Authorizing access to health data

## Discussion

This method checks the authorization status for saving data to the HealthKit store.

Important

An app’s permissions don’t change when an app runs in a Guest User session. Therefore, authorizationStatus(for:) returns true if the owner previously granted authorization to write the data, even though the app can’t write it during a Guest User session. For more information, refer to Authorizing access to health data.

To help prevent possible leaks of sensitive health information, your app cannot determine whether or not a user has granted permission to read data. If you are not given permission, it simply appears as if there is no data of the requested type in the HealthKit store. If your app is given share permission but not read permission, you see only the data that your app has written to the store. Data from other sources remains hidden.

## See Also

### Accessing HealthKit

enum HKAuthorizationStatus

Constants indicating the authorization status for a particular data type.

func getRequestStatusForAuthorization(toShare: Set&lt;HKSampleType>, read: Set&lt;HKObjectType>, completion: (HKAuthorizationRequestStatus, (any Error)?) -> Void)

Indicates whether the system presents the user with a permission sheet if your app requests authorization for the provided types.

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

