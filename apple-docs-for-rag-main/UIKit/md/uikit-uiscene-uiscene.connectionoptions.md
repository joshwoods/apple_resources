

- UIKit
- UIScene
-  UIScene.ConnectionOptions 

Class

# UIScene.ConnectionOptions

A data object containing information about the reasons why UIKit created the scene.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class ConnectionOptions
```

## Overview

UIKit creates scenes for many reasons. It might do so in response to a Handoff request or a request to open a URL. When there’s a specific reason for creating a scene, UIKit fills a UIScene.ConnectionOptions object with the associated data and passes it to your delegate at connection time. Use the information in this object to respond accordingly. For example, open the URLs that UIKit provides, and display their contents in the scene.

Don’t create UIScene.ConnectionOptions objects directly. UIKit creates UIScene.ConnectionOptions objects for you and passes them to the scene(_:willConnectTo:options:) method of your scene delegate.

## Topics

### Configuring the scene’s interface

var userActivities: Set&lt;NSUserActivity>

Information about user activities that you can use to configure your scene’s interface.

### Handling quick actions

var shortcutItem: UIApplicationShortcutItem?

The user-selected action to perform.

### Opening URLs

var urlContexts: Set&lt;UIOpenURLContext>

The URLs to open, along with metadata specifying how to open them.

### Responding to a Handoff request

var handoffUserActivityType: String?

The type of the pending Handoff activity.

### Accepting a CloudKit share

var cloudKitShareMetadata: CKShareMetadata?

Information about the CloudKit data that’s now available to the app.

### Responding to notifications

var notificationResponse: UNNotificationResponse?

A person’s response to one of your app’s notifications.

### Preparing for Near-Field Communication (NFC)

var nfcEvent: NFCWindowSceneEvent?

An event, such as a gesture or exposure to a card reader’s RF field, that creates a Near-Field Communication (NFC) scene.

### Getting the source app

var sourceApplication: String?

The bundle ID of the app that originated the request.

### Instance Properties

var credentialSessionEvent: CredentialSessionWindowSceneEvent?

A CredentialSession event has triggered a UIKit scene creation.

var gameControllerActivationContext: GCGameControllerActivationContext?

var marketplaceDisplayOption: MarketplaceDisplayOption?

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Connecting and disconnecting the scene

func scene(UIScene, willConnectTo: UISceneSession, options: UIScene.ConnectionOptions)

Tells the delegate about the addition of a scene to the app.

func sceneDidDisconnect(UIScene)

Tells the delegate that UIKit removed a scene from your app.

