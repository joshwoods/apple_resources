

- UIKit
- UIApplication
- UIApplication.LaunchOptionsKey
-  annotation Deprecated

Type Property

# annotation

A key indicating that the URL passed to your app contained custom annotation data from the source app.

iOS 3.2–16.0DeprecatediPadOS 3.2–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedtvOSDeprecated

``` source
static let annotation: UIApplication.LaunchOptionsKey
```

## Discussion

The presence of this key indicates that custom data was provided by the app that requested the opening of the URL. The value of this key is a property-list object containing the custom data. The same object is also passed to the annotation parameter of the application(_:open:sourceApplication:annotation:) method. The contents of this property-list object are specific to the app that made the request.

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

static let localNotification: UIApplication.LaunchOptionsKey

A key indicating that the app was launched to handle a local notification.

Deprecated

