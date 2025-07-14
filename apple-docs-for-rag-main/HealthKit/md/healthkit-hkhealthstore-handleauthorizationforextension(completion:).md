

- HealthKit
- HKHealthStore
-  handleAuthorizationForExtension(completion:) 

Instance Method

# handleAuthorizationForExtension(completion:)

Requests permission to save and read the data types specified by an extension.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+

``` source
func handleAuthorizationForExtension(completion: @escaping (Bool, (any Error)?) -> Void)
```

``` source
func handleAuthorizationForExtension() async throws
```

## Parameters 

`completion`  

A block that is called after the user finishes responding to the request. This block is passed the following parameters:

success  
A Boolean value that indicates whether the user responded to the prompt (if any). This value does not indicate whether permission was actually granted. This parameter is false if the user canceled the prompt without selecting permissions; otherwise, true.

error  
An error object. If an error occurred, this object contains information about the error; otherwise, it is set to `nil`.

## Discussion

The host app must implement the application delegate’s applicationShouldRequestHealthAuthorization(_:) method. This delegate method is called after an app extension calls requestAuthorization(toShare:read:completion:). The host app is then responsible for calling handleAuthorizationForExtension(completion:). This method prompts the user to authorize both the app and its extensions for the types that the extension requested.

The system performs this request asynchronously. After the user has finished responding, this method calls its completion block on a background queue. If the user has already chosen to grant or prohibit access to all of the types specified, the completion is called without prompting the user.

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

func requestPerObjectReadAuthorization(for: HKObjectType, predicate: NSPredicate?, completion: (Bool, (any Error)?) -> Void)

Asynchronously requests permission to read a data type that requires per-object authorization (such as vision prescriptions).

var authorizationViewControllerPresenter: UIViewController?

The view controller that presents HealthKit authorization sheets.

