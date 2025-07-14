

- User Notifications UI
-  UNNotificationContentExtension 

Protocol

# UNNotificationContentExtension

An object that presents a custom interface for a delivered local or remote notification.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+macOS 11.0+visionOS 1.0+

``` source
protocol UNNotificationContentExtension : NSObjectProtocol
```

## Mentioned in 

Customizing the Appearance of Notifications

## Overview

The `UNNotificationContentExtension` protocol provides the entry point for a notification content app extension, which displays a custom interface for your app’s notifications. You adopt this protocol in the custom UIViewController subclass that you use to present your interface. You create this type of extension to improve the way your notifications are presented, possibly by adding custom colors and branding, or by incorporating media and other dynamic content into your notification interface.

To define a notification content app extension, add a notification content extension target to the Xcode project containing your app. The default Xcode template contains a source file and storyboard for your view controller. The `Info.plist` file of the extension comes mostly configured. Specifically, the `NSExtensionPointIdentifier` key is set to the value `com.apple.usernotifications.content-extension`, and the `NSExtensionMainStoryboard` key is set to the name of the project’s storyboard file. However, the `NSExtensionAttribute` key contains a dictionary of additional keys and values, which are listed in the following table.

| Key | Value |
|----|----|
| `UNNotificationExtensionCategory` (Required) | A string or an array of strings. Each string contains the identifier of a category declared by the app using the UNNotificationCategory class. |
| `UNNotificationExtensionInitialContentSizeRatio` (Required) | A floating-point number that represents the initial size of your view controller’s view expressed as a ratio of its height to its width. The system uses this value to set the initial size of the view controller while your extension is loading. For example, a value of 0.5 results in a view controller whose height is half its width. You can change the size of your view controller after your extension loads. |
| `UNNotificationExtensionDefaultContentHidden` | A Boolean. When set to YES, the system displays only your custom view controller in the notification interface. When set to NO, the system displays the default notification content in addition to your view controller’s content. Custom action buttons and the Dismiss button are always displayed, regardless of this setting. If you don’t specify this key, the default value is set to NO. |
| `UNNotificationExtensionOverridesDefaultTitle` | A Boolean. When set to YES, the system uses the title property of your view controller as the title of the notification. When set to NO, the system sets the notification’s title to the name of your app. If you don’t specify this key, the default value is set to NO. |

If the notification category includes custom actions, the system automatically adds action buttons to your notification interface; don’t create those buttons yourself. If your view controller implements the optional didReceive(_:completionHandler:) method, the system calls that method to respond to any selected actions. If your view controller doesn’t implement that method, the system delivers the selected action to your app for handling.

The system prevents the delivery of touch events to your view controller while it is onscreen. Do not install gesture recognizers or rely on touch events in your interface.

For information about how to implement your notification content app extension, see Customizing the Appearance of Notifications.

## Topics

### Processing Notifications

func didReceive(UNNotification)

Delivers a new notification to your notification content app extension.

**Required**

### Handling Custom Actions

func didReceive(UNNotificationResponse, completionHandler: (UNNotificationContentExtensionResponseOption) -> Void)

Handles a notification action selected by the user.

enum UNNotificationContentExtensionResponseOption

Constants indicating the preferred response to a notification.

### Supporting Media Playback

var mediaPlayPauseButtonType: UNNotificationContentExtensionMediaPlayPauseButtonType

The type of media button type to display.

enum UNNotificationContentExtensionMediaPlayPauseButtonType

Constants indicating the type of media button to display.

var mediaPlayPauseButtonFrame: CGRect

The frame rectangle to use for displaying a media playback button.

var mediaPlayPauseButtonTintColor: UIColor

The tint color for the media playback button.

func mediaPlay()

Tells you to begin playback of your media content.

func mediaPause()

Tells you to pause playback of your media content.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Related Documentation

Scheduling a notification locally from your app

Create and schedule notifications from your app when you want to get the user’s attention.

Setting up a remote notification server

Generate notifications and push them to user devices.

### Notification Content App Extension

Customizing the Appearance of Notifications

Customize the appearance of your iOS app’s notification alerts with a notification content app extension.

