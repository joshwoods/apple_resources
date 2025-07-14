

- User Notifications
-  UNMutableNotificationContent 

Class

# UNMutableNotificationContent

The editable content for a notification.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class UNMutableNotificationContent
```

## Mentioned in 

Declaring your actionable notification types

Modifying content in newly delivered notifications

## Overview

Create a UNMutableNotificationContent object when you want to specify the payload for a local notification. Specifically, use this object to specify the title and message for an alert, the sound to play, or the value to assign to your app’s badge. You might also provide details about how the system handles the notification. For example, you can specify a custom launch image and a thread identifier for visually grouping related notifications.

After creating your content object, assign it to a UNNotificationRequest object, add a trigger condition, and schedule your notification. The trigger condition defines when the system delivers the notification to the user. Listing 1 shows the scheduling of a local notification that displays an alert and plays a sound after a delay of five seconds. Store the strings for the alert’s title and body in the app’s `Localizable.strings` file.

Listing 1. Creating the content for a local notification

- Swift
- Objective-C

```
// Configure the notification's payload.
let content = UNMutableNotificationContent()
content.title = NSString.localizedUserNotificationStringForKey("Hello!", arguments: nil)
content.body = NSString.localizedUserNotificationStringForKey("Hello_message_body", arguments: nil)
content.sound = UNNotificationSound.default()

// Deliver the notification in five seconds.
let trigger = UNTimeIntervalNotificationTrigger(timeInterval: 5, repeats: false)
let request = UNNotificationRequest(identifier: "FiveSecond", content: content, trigger: trigger) // Schedule the notification.
let center = UNUserNotificationCenter.current()
center.add(request) { (error : Error?) in
     if let theError = error {
         // Handle any errors
     }
}
```

```
// Configure the notification's payload.
UNMutableNotificationContent *content = [[UNMutableNotificationContent alloc] init];
content.title = [NSString localizedUserNotificationStringForKey:@"Hello!" arguments:nil];
content.body = [NSString localizedUserNotificationStringForKey:@"Hello_message_body"
            arguments:nil];
content.sound = [UNNotificationSound defaultSound];

// Deliver the notification in five seconds.
UNTimeIntervalNotificationTrigger* trigger = [UNTimeIntervalNotificationTrigger
            triggerWithTimeInterval:5 repeats:NO];
UNNotificationRequest* request = [UNNotificationRequest requestWithIdentifier:@"FiveSecond"
            content:content trigger:trigger];

// Schedule the notification.
UNUserNotificationCenter* center = [UNUserNotificationCenter currentNotificationCenter];
[center addNotificationRequest:request];
```

Note

Local notifications always result in user interactions, and the system ignores any interactions for which your app isn’t authorized. For information about how to request authorization for user interactions, see Asking permission to use notifications.

### Localizing the Alert Strings

Localize the strings you display in a notification alert for the current user. Although you can use the NSLocalizedString macros to load strings from your app’s resource files, a better option is to specify your string using the localizedUserNotificationString(forKey:arguments:) method of NSString. The localizedUserNotificationString(forKey:arguments:) method delays the loading of the localized string until the system delivers the notification. If the user changes the language setting before the system delivers a notification, the system updates the alert text to the user’s current language instead of the language in use when the system scheduled the notification.

## Topics

### Providing the primary content

var title: String

The localized text that provides the notification’s primary description.

var subtitle: String

The localized text that provides the notification’s secondary description.

var body: String

The localized text that provides the notification’s main content.

### Providing supplementary content

var attachments: [UNNotificationAttachment]

The visual and audio attachments to display alongside the notification’s main content.

var userInfo: [AnyHashable : Any]

The custom data to associate with the notification.

### Configuring app behavior

var launchImageName: String

The name of the image or storyboard to use when your app launches because of the notification.

var badge: NSNumber?

The number that your app’s icon displays.

var targetContentIdentifier: String?

The value your app uses to determine which scene to display to handle the notification.

### Integrating with the system

var sound: UNNotificationSound?

The sound that plays when the system delivers the notification.

var interruptionLevel: UNNotificationInterruptionLevel

The notification’s importance and required delivery timing.

enum UNNotificationInterruptionLevel

Constants that indicate the importance and delivery timing of a notification.

var relevanceScore: Double

The score the system uses to determine if the notification is the summary’s featured notification.

var filterCriteria: String?

The criteria the system evaluates to determine if it displays the notification in the current Focus.

### Grouping notifications

var threadIdentifier: String

The identifier that groups related notifications.

var categoryIdentifier: String

The identifier of the notification’s category.

var summaryArgument: String

The text the system adds to the notification summary to provide additional context.

Deprecated

var summaryArgumentCount: Int

The number the system adds to the notification summary when the notification represents multiple items.

Deprecated

## Relationships

### Inherits From

- UNNotificationContent

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSMutableCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Notification content

Implementing communication notifications

Configure and display your app’s communication notifications by using intents.

protocol UNNotificationContentProviding

A protocol the system uses to provide context relevant to user notifications.

class UNNotificationActionIcon

An icon associated with an action.

class UNNotificationContent

The uneditable content of a notification.

class UNNotificationAttachment

A media file associated with a notification.

class UNNotificationSound

The sound played upon delivery of a notification.

struct UNNotificationSoundName

A string providing the name of a sound file.

