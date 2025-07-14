

- UIKit
- UIApplication
- UIApplication.LaunchOptionsKey
-  bluetoothCentrals 

Type Property

# bluetoothCentrals

A key indicating that the app was relaunched to handle Bluetooth-related events.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
static let bluetoothCentrals: UIApplication.LaunchOptionsKey
```

## Discussion

The presence of this key indicates that the app previously had one or more CBCentralManager objects and was relaunched by the Bluetooth system to continue actions associated with those objects. The value of this key is an NSArray object containing one or more NSString objects.

Each string in the array represents the restoration identifier for a central manager object. This is the same string you assigned to the CBCentralManagerOptionRestoreIdentifierKey key when you initialized the central manager object previously. The system provides the restoration identifiers only for central managers that had active or pending peripheral connections or were scanning for peripherals.

## See Also

### Accessing launch options

static let bluetoothPeripherals: UIApplication.LaunchOptionsKey

A key indicating that the app should continue actions associated with its Bluetooth peripheral objects.

static let cloudKitShareMetadata: UIApplication.LaunchOptionsKey

A key indicating that the app received a CloudKit share invitation.

static let eventAttribution: UIApplication.LaunchOptionsKey

static let location: UIApplication.LaunchOptionsKey

A key indicating that the app was launched to handle an incoming location event.

static let newsstandDownloads: UIApplication.LaunchOptionsKey

A key indicating that the app was launched to process newly downloaded Newsstand assets.

static let remoteNotification: UIApplication.LaunchOptionsKey

A key indicating that a remote notification is available for the app to process.

static let shortcutItem: UIApplication.LaunchOptionsKey

A key indicating that the app was launched in response to the user selecting a Home screen quick action.

static let sourceApplication: UIApplication.LaunchOptionsKey

A key indicating that another app requested the launch of your app.

static let url: UIApplication.LaunchOptionsKey

A key indicating that the app was launched so that it could open the specified URL.

static let userActivityDictionary: UIApplication.LaunchOptionsKey

A key indicating a dictionary associated with an activity that the user wants to continue.

static let userActivityType: UIApplication.LaunchOptionsKey

A key indicating the type of user activity that the user wants to continue.

static let annotation: UIApplication.LaunchOptionsKey

A key indicating that the URL passed to your app contained custom annotation data from the source app.

Deprecated

static let localNotification: UIApplication.LaunchOptionsKey

A key indicating that the app was launched to handle a local notification.

Deprecated

