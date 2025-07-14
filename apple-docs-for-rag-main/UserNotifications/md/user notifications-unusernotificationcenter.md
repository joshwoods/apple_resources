

- User Notifications
-  UNUserNotificationCenter 

Class

# UNUserNotificationCenter

The central object for managing notification-related activities for your app or app extension.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class UNUserNotificationCenter
```

## Mentioned in 

Handling notifications and notification-related actions

Asking permission to use notifications

Declaring your actionable notification types

## Overview

Use the shared UNUserNotificationCenter object to manage all notification-related behaviors in your app or app extension. Specifically, use this object to do the following:

- Request authorization to interact with the user through alerts, sounds, and icon badges. See Asking permission to use notifications.

- Declare the notification types that your app supports and the custom actions the user may perform when the system delivers those notifications. See Declaring your actionable notification types.

- Schedule the delivery of notifications from your app. See Scheduling a notification locally from your app.

- Process the payloads from remote notifications the system delivers by Apple Push Notification service (APNs). See Handling notifications and notification-related actions.

- Manage the already delivered notifications the system displays in Notification Center. See Managing Delivered Notifications.

- Handle user-selected actions associated with your custom notification types. See Handling notifications and notification-related actions.

- Get the notification-related settings for your app. See Managing Settings and Authorization.

To handle incoming notifications and notification-related actions, create an object that adopts the UNUserNotificationCenterDelegate protocol and assign it to the delegate property. Always assign an object to the delegate property before performing any tasks that might interact with that delegate.

You may use the shared user notification center object simultaneously from any of your app’s threads. The object processes requests serially in the order that the system initiates them.

## Topics

### Managing the notification center

class func current() -> UNUserNotificationCenter

Returns your app’s notification center.

func getNotificationSettings(completionHandler: (UNNotificationSettings) -> Void)

Retrieves the authorization and feature-related settings for your app.

func setBadgeCount(Int, withCompletionHandler: (((any Error)?) -> Void)?)

Updates the badge count for your app’s icon.

### Requesting authorization

func requestAuthorization(options: UNAuthorizationOptions, completionHandler: (Bool, (any Error)?) -> Void)

Requests a person’s authorization to allow local and remote notifications for your app.

struct UNAuthorizationOptions

Options that determine the authorized features of local and remote notifications.

### Processing received notifications

var delegate: (any UNUserNotificationCenterDelegate)?

The notification center’s delegate.

protocol UNUserNotificationCenterDelegate

An interface for processing incoming notifications and responding to notification actions.

var supportsContentExtensions: Bool

A Boolean value that indicates whether the device supports notification content extensions.

### Scheduling notifications

func add(UNNotificationRequest, withCompletionHandler: (((any Error)?) -> Void)?)

Schedules the delivery of a local notification.

func getPendingNotificationRequests(completionHandler: ([UNNotificationRequest]) -> Void)

Fetches all of your app’s local notifications that are pending delivery.

func removePendingNotificationRequests(withIdentifiers: [String])

Removes your app’s local notifications that are pending and match the specified identifiers.

func removeAllPendingNotificationRequests()

Removes all of your app’s pending local notifications.

### Removing delivered notifications

func getDeliveredNotifications(completionHandler: ([UNNotification]) -> Void)

Fetches all of your app’s delivered notifications that are still present in Notification Center.

func removeDeliveredNotifications(withIdentifiers: [String])

Removes your app’s notifications from Notification Center that match the specified identifiers.

func removeAllDeliveredNotifications()

Removes all of your app’s delivered notifications from Notification Center.

### Managing notification categories

func setNotificationCategories(Set&lt;UNNotificationCategory>)

Registers the notification categories that your app supports.

func getNotificationCategories(completionHandler: (Set&lt;UNNotificationCategory>) -> Void)

Fetches your app’s registered notification categories.

### Handling errors

struct UNError

An object that represents a notification error.

enum Code

Constants that identify notification errors.

let UNErrorDomain: String

The error domain for notifications.

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

## See Also

### Notification management

protocol UNUserNotificationCenterDelegate

An interface for processing incoming notifications and responding to notification actions.

class UNNotificationSettings

The object for managing notification-related settings and the authorization status of your app.

