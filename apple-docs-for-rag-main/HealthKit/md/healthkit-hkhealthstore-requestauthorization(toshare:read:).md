

- HealthKit
- HKHealthStore
-  requestAuthorization(toShare:read:) 

Instance Method

# requestAuthorization(toShare:read:)

Asynchronously requests permission to save and read the specified data types.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 13.0+visionOSwatchOS 8.0+

``` source
func requestAuthorization(
    toShare typesToShare: Set,
    read typesToRead: Set
) async throws
```

## Parameters 

`typesToShare`  

A set containing the data types you want to share. This set can contain any concrete subclass of the HKSampleType class (any of the HKQuantityType, HKCategoryType, HKWorkoutType, or HKCorrelationType classes). If the user grants permission, your app can create and save these data types to the HealthKit store.

`typesToRead`  

A set containing the data types you want to read. This set can contain any concrete subclass of the HKObjectType class (any of the HKCharacteristicType , HKQuantityType, HKCategoryType, HKWorkoutType, or HKCorrelationType classes ). If the user grants permission, your app can read these data types from the HealthKit store.

## Mentioned in 

Authorizing access to health data

## Discussion

HealthKit performs these requests asynchronously. If you call this method with a new data type (a type of data that the user hasn’t previously granted or denied permission for in this app), the system automatically displays the permission form, listing all the requested permissions. After the user has finished responding, this method calls its completion block on a background queue. If the user has already chosen to grant or prohibit access to all of the types specified, HealthKit calls the completion without prompting the user.

Important

In watchOS 6 and later, this method displays the permission form on Apple Watch, enabling independent HealthKit apps. In watchOS 5 and earlier, this method prompts the user to authorize the app on their paired iPhone. For more information, see `Creating Independent watchOS Apps`.

Each data type has two separate permissions, one to read it and one to share it. You can make a single request, and include all the data types your app needs.

Customize the messages displayed on the permissions sheet by setting the following keys:

- NSHealthShareUsageDescription customizes the message for reading data.

- NSHealthUpdateUsageDescription customizes the message for writing data.

Warning

You must set the usage keys, or your app will crash when you request authorization.

For projects created using Xcode 13 or later, set these keys in the Target Properties list on the app’s Info tab. For projects created with Xcode 12 or earlier, set these keys in the apps `Info.plist` file. For more information, see Information Property List.

After users have set the permissions for your app, they can always change them using either the Settings or the Health app. Your app appears in the Health app’s Sources tab, even if the user didn’t allow permission to read or share data.

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

func requestPerObjectReadAuthorization(for: HKObjectType, predicate: NSPredicate?, completion: (Bool, (any Error)?) -> Void)

Asynchronously requests permission to read a data type that requires per-object authorization (such as vision prescriptions).

func handleAuthorizationForExtension(completion: (Bool, (any Error)?) -> Void)

Requests permission to save and read the data types specified by an extension.

var authorizationViewControllerPresenter: UIViewController?

The view controller that presents HealthKit authorization sheets.

