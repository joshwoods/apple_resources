

- UIKit
- UIApplication
-  UIApplication.LaunchOptionsKey 

Structure

# UIApplication.LaunchOptionsKey

The keys you use to access values in the launch options dictionary that the system passes to your app at initialization.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
struct LaunchOptionsKey
```

## Overview

These keys are passed to the options dictionary that’s passed to the application(_:willFinishLaunchingWithOptions:) and application(_:didFinishLaunchingWithOptions:) methods of the app delegate.

## Topics

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

static let annotation: UIApplication.LaunchOptionsKey

A key indicating that the URL passed to your app contained custom annotation data from the source app.

Deprecated

static let localNotification: UIApplication.LaunchOptionsKey

A key indicating that the app was launched to handle a local notification.

Deprecated

### Creating a launch options key

init(rawValue: String)

Creates a launch options key with the specified raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Initializing the app

func application(UIApplication, willFinishLaunchingWithOptions: [UIApplication.LaunchOptionsKey : Any]?) -> Bool

Tells the delegate that the launch process has begun.

func application(UIApplication, didFinishLaunchingWithOptions: [UIApplication.LaunchOptionsKey : Any]?) -> Bool

Tells the delegate that the launch process is almost done and the app is almost ready to run.

class let didFinishLaunchingNotification: NSNotification.Name

A notification that posts immediately after the app finishes launching.

