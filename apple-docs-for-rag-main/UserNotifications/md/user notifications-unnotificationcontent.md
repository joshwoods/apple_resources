

- User Notifications
-  UNNotificationContent 

Class

# UNNotificationContent

The uneditable content of a notification.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class UNNotificationContent
```

## Mentioned in 

Generating a remote notification

## Overview

A UNNotificationContent object contains the data associated with a notification. When your app receives a notification, the associated UNNotificationRequest object contains an object of this type with the content that your app received. Use the content object to get the details of the notification, including the type of notification that the system delivered, any custom data you stored in the userInfo dictionary before scheduling the notification, and any attachments.

Don’t create instances of this class directly. For remote notifications, the system derives the contents of this object from the JSON payload that your server sends to the APNS server. For local notifications, create a UNMutableNotificationContent object, and configure the contents of that object instead.

## Topics

### Accessing the primary content

var title: String

The localized text that provides the notification’s primary description.

var subtitle: String

The localized text that provides the notification’s secondary description.

var body: String

The localized text that provides the notification’s main content.

### Accessing supplementary content

var attachments: [UNNotificationAttachment]

The visual and audio attachments to display alongside the notification’s main content.

var userInfo: [AnyHashable : Any]

The custom data to associate with the notification.

### Reading app configuration

var launchImageName: String

The name of the image or storyboard to use when your app launches because of the notification.

var badge: NSNumber?

The number that your app’s icon displays.

var targetContentIdentifier: String?

The value your app uses to determine which scene to display to handle the notification.

### Reading system configuration

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

### Retrieving group information

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

### Updating the notification’s content

func updating(from: any UNNotificationContentProviding) throws -> UNNotificationContent

Returns a copy of the notification that includes content from the specified provider.

## Relationships

### Inherits From

- NSObject

### Inherited By

- UNMutableNotificationContent

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

class UNMutableNotificationContent

The editable content for a notification.

class UNNotificationAttachment

A media file associated with a notification.

class UNNotificationSound

The sound played upon delivery of a notification.

struct UNNotificationSoundName

A string providing the name of a sound file.

