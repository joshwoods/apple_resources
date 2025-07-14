

- HealthKit
- HKHealthStore
-  requestPerObjectReadAuthorization(for:predicate:completion:) 

Instance Method

# requestPerObjectReadAuthorization(for:predicate:completion:)

Asynchronously requests permission to read a data type that requires per-object authorization (such as vision prescriptions).

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
func requestPerObjectReadAuthorization(
    for objectType: HKObjectType,
    predicate: NSPredicate?,
    completion: @escaping (Bool, (any Error)?) -> Void
)
```

``` source
func requestPerObjectReadAuthorization(
    for objectType: HKObjectType,
    predicate: NSPredicate?
) async throws
```

## Parameters 

`objectType`  

The data type you want to read.

`predicate`  

A predicate that further restricts the data type.

`completion`  

A completion handler that the system calls after the user responds to the request. The completion handler has the following parameters:

success  
A Boolean value that indicates whether the request succeeded. This value doesn’t indicate whether the user actually granted permission. The parameter is false if an error occurred while processing the request; otherwise, it’s true.

error  
An error object. If an error occurred, this object contains information about the error; otherwise, the system passes `nil`.

## Discussion

Some samples require per-object authorization. For these samples, people can select which ones your app can read on a sample-by-sample basis. By default, your app can read any of the per-object authorization samples that it has saved to the HealthKit store; however, you may not always have access to those samples. People can update the authorization status for any of these samples at any time.

Your app can begin by querying for any samples that it already has permission to read.

```
// Read the newest prescription from the HealthKit store.
let queryDescriptor = HKSampleQueryDescriptor(predicates: [.visionPrescription()],
  sortDescriptors: [SortDescriptor(\.startDate, order: .reverse)],
  limit: 1)

let prescription: HKVisionPrescription

do {
guard let result = try await queryDescriptor.result(for: store).first else {
print("*** No prescription found. ***")
return
}

prescription = result
} catch {
// Handle the error here.
fatalError("*** An error occurred while reading the most recent vision prescriptions: \(error.localizedDescription) ***")
}
```

Based on the results, you can then decide whether you need to request authorization for additional samples. Call requestPerObjectReadAuthorization(for:predicate:completion:) to prompt someone to modify the samples your app has access to read.

```
// Request authorization to read vision prescriptions.
do {
try await store.requestPerObjectReadAuthorization(for: .visionPrescriptionType(),
  predicate: nil)
} catch HKError.errorUserCanceled {
// Handle the user canceling the authorization request.
print("*** The user canceled the authorization request. ***")
return
} catch {
// Handle the error here.
fatalError("*** An error occurred while requesting permission to read vision prescriptions: \(error.localizedDescription) ***")
}
```

Important

Using the requestAuthorization(toShare:read:) method to request read access to any data types that require per-object authorization fails with an HKError.Code.errorInvalidArgument error.

When your app calls this method, HealthKit displays an authorization sheet that asks for permission to read the samples that match the predicate and object type. The person using your app can then select individual samples to share with your app. The system always asks for permission, regardless of whether they previously granted it.

After the person responds, the system calls the callback handler on an arbitrary background queue.

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

class func isHealthDataAvailable() -> Bool

Returns a Boolean value that indicates whether HealthKit is available on this device.

func supportsHealthRecords() -> Bool

Returns a Boolean value that indicates whether the current device supports clinical records.

func requestAuthorization(toShare: Set&lt;HKSampleType>?, read: Set&lt;HKObjectType>?, completion: (Bool, (any Error)?) -> Void)

Requests permission to save and read the specified data types.

func requestAuthorization(toShare: Set&lt;HKSampleType>, read: Set&lt;HKObjectType>) async throws

Asynchronously requests permission to save and read the specified data types.

func handleAuthorizationForExtension(completion: (Bool, (any Error)?) -> Void)

Requests permission to save and read the data types specified by an extension.

var authorizationViewControllerPresenter: UIViewController?

The view controller that presents HealthKit authorization sheets.

