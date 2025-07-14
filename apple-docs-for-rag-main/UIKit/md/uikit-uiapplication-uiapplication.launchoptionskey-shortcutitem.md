

- UIKit
- UIApplication
- UIApplication.LaunchOptionsKey
-  shortcutItem 

Type Property

# shortcutItem

A key indicating that the app was launched in response to the user selecting a Home screen quick action.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
static let shortcutItem: UIApplication.LaunchOptionsKey
```

## Discussion

The value of this key is the UIApplicationShortcutItem object representing the action that the user selected.

## See Also

### Accessing launch options

static let bluetoothCentrals: UIApplication.LaunchOptionsKey

A key indicating that the app was relaunched to handle Bluetooth-related events.

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

