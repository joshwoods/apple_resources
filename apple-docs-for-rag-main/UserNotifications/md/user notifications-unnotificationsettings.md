

- User Notifications
-  UNNotificationSettings 

Class

# UNNotificationSettings

The object for managing notification-related settings and the authorization status of your app.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class UNNotificationSettings
```

## Mentioned in 

Asking permission to use notifications

## Overview

A UNNotificationSettings object contains the current authorization status and notification-related settings for your app. Apps must receive authorization to schedule notifications and to interact with the user. Apps that run in CarPlay must similarly receive authorization to do so. Use this object to determine what notification-related actions your app can perform. You might then use that information to enable, disable, or adjust your app’s notification-related behaviors. Regardless of whether you take action, the system enforces your app’s settings by preventing denied interactions from occurring.

You don’t create instances of this class directly. Instead, call the getNotificationSettings(completionHandler:) method of your app’s UNUserNotificationCenter object to get the current settings.

For more information about requesting authorization for user interactions, see UNUserNotificationCenter.

## Topics

### Getting the Authorization Status

var authorizationStatus: UNAuthorizationStatus

The app’s ability to schedule and receive local and remote notifications.

enum UNAuthorizationStatus

Constants indicating whether the app is allowed to schedule notifications.

### Getting Device-Specific Settings

var notificationCenterSetting: UNNotificationSetting

The setting that indicates whether your app’s notifications appear in Notification Center.

var lockScreenSetting: UNNotificationSetting

The setting that indicates whether your app’s notifications appear on a device’s Lock screen.

var carPlaySetting: UNNotificationSetting

The setting that indicates whether your app’s notifications appear in CarPlay.

var alertSetting: UNNotificationSetting

The authorization status for displaying alerts.

var badgeSetting: UNNotificationSetting

The setting that indicates whether badges appear on your app’s icon.

var soundSetting: UNNotificationSetting

The authorization status for playing sounds for incoming notifications.

var criticalAlertSetting: UNNotificationSetting

The authorization status for playing sounds for critical alerts.

var announcementSetting: UNNotificationSetting

The setting that indicates whether Siri can announce your app’s notifications.

var scheduledDeliverySetting: UNNotificationSetting

The setting that indicates the system schedules the notification.

var timeSensitiveSetting: UNNotificationSetting

The setting that indicates the system treats the notification as time-sensitive.

enum UNNotificationSetting

Constants that indicate the current status of a notification setting.

### Getting Interface Settings

var alertStyle: UNAlertStyle

The type of alert that the app may display when the device is unlocked.

enum UNAlertStyle

Constants indicating the presentation styles for alerts.

var showPreviewsSetting: UNShowPreviewsSetting

The setting that indicates whether the app shows a preview of the notification’s content.

enum UNShowPreviewsSetting

Constants indicating the style previewing a notification’s content.

var providesAppNotificationSettings: Bool

A Boolean value indicating the system displays a button for in-app notification settings.

### Instance Properties

var directMessagesSetting: UNNotificationSetting

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Notification management

class UNUserNotificationCenter

The central object for managing notification-related activities for your app or app extension.

protocol UNUserNotificationCenterDelegate

An interface for processing incoming notifications and responding to notification actions.

