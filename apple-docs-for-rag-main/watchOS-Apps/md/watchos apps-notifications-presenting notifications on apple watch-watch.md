

- watchOS apps
- Notifications
-  Presenting notifications on Apple Watch 

Article

# Presenting notifications on Apple Watch

Understand how the system displays incoming notifications.

## Overview

When the Apple Watch displays a notification, the system first presents the short-look interface. If the user continues to look at the notification, the system transitions quickly from the short-look interface to the long-look interface

### Display a short-look interface

The *short-look* interface is a nonscrolling screen that the system creates automatically.

The system uses a template to display the app name and icon along with the title string from the notification payload, and you can’t customize this interface. For local notifications, you specify the title string using the UNMutableNotificationContent object’s title property. For remote notifications, you specify it using the `alert` dictionary’s `title` key inside the notification’s payload.

### Transition to the long-look interface

The *long-look* interface is a scrollable screen that displays the notification’s content and any associated action buttons. The system’s default long-look interface includes your app icon, the notification’s title string, and the alert message; however, your app can customize this interface.

The long-look notification includes the following sections:

- The sash is an overlay that contains the app icon and app name. The system automatically generates the sash, but you can configure the appearance using the hosting controller’s sashColor, titleColor, subtitleColor, and wantsSashBlur properties.

- The content area contains detailed information about the incoming notification. If you provide a dynamic interactive interface for the notification, the content area can contain controls, like buttons or switches. For information on customizing the long-look interface, see Customizing your long-look interface.

- The bottom contains a Dismiss button and any registered action buttons. For more information, see Adding actions to notifications on watchOS.

By default, the system dismisses the long-look interface, launches your app, and calls your notification center delegate’s userNotificationCenter(_:didReceive:withCompletionHandler:) method when the user taps the notification. The response parameter’s actionIdentifier property varies, as shown below.

| Interface element | Action identifier |
|----|----|
| Action button | The identifier for the selected action |
| Dismiss button | UNNotificationDismissActionIdentifier |
| Anywhere else | UNNotificationDefaultActionIdentifier |

For dynamic interactive interfaces, tapping the app content doesn’t launch your watchOS app. Instead, the user can interact with any controls placed in the interface, and the system calls the corresponding action method. The system only dismisses the notification and launches your app if the user taps the app icon or sash, or if you explicitly call the notification controller’s performNotificationDefaultAction() method.

## See Also

### Essentials

Enabling and receiving notifications

Set up and handle local and remote notifications.

