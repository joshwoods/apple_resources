

- User Notifications
-  UNNotificationAttachment 

Class

# UNNotificationAttachment

A media file associated with a notification.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
class UNNotificationAttachment
```

## Overview

Create a UNNotificationAttachment object when you want to include audio, image, or video content together in an alert-based notification. When creating the UNNotificationAttachment object, the file you specify must be on disk, and the file format must be one of the supported types.

You’re responsible for supplying attachments before the system displays your notification’s alert. For local notifications, add attachments when creating the notification’s content. For remote notifications, use a notification service app extension to download the attached files and then add them to the notification’s content before delivery.

The system validates attachments before displaying the associated notification. If you attach a file to a local notification request that’s corrupted, invalid, or of an unsupported file type, the system doesn’t schedule your request. For remote notifications, the system validates attachments after your notification service app extension finishes. Once validated, the system moves the attached files into the attachment data store so that the appropriate processes can access the files. The system copies attachments located inside an app’s bundle.

### Supported File Types

Table 1 lists the types of files you can include as an attachment and the supported file formats. The table also lists the maximum size allowed for attachments of each type. An image file may contain a static image or an animated image sequence.

Table 1. Supported attachment file types

| Attachment | Supported file types | Maximum size |
|----|----|----|
| Audio | `kUTTypeAudioInterchangeFileFormat`  `kUTTypeWaveformAudio`  `kUTTypeMP3`  `kUTTypeMPEG4Audio` | 5 MB |
| Image | `kUTTypeJPEG`  `kUTTypeGIF`  `kUTTypePNG` | 10 MB |
| Movie | `kUTTypeMPEG`  `kUTTypeMPEG2Video`  `kUTTypeMPEG4`  `kUTTypeAVIMovie` | 50 MB |

When creating an attachment, you can specify optional details about how to present the thumbnail image for the image or movie. Use the UNNotificationAttachmentOptionsThumbnailClippingRectKey option to use only the specified portion of an image as a thumbnail. For animated images and movies, use the UNNotificationAttachmentOptionsThumbnailTimeKey option to select which frame to use for the thumbnail image.

The system limits the amount of storage space allocated for attachments for each app. To delete attachments, use the methods of the UNUserNotificationCenter class to remove the notification requests that contain those attachments.

## Topics

### Creating an Attachment

convenience init(identifier: String, url: URL, options: [AnyHashable : Any]?) throws

Creates an attachment object from the specified file and options.

let UNNotificationAttachmentOptionsTypeHintKey: String

A hint about an attachment’s file type.

let UNNotificationAttachmentOptionsThumbnailHiddenKey: String

A Boolean value indicating whether the system hides the attachment’s thumbnail.

let UNNotificationAttachmentOptionsThumbnailClippingRectKey: String

The clipping rectangle for a thumbnail image.

let UNNotificationAttachmentOptionsThumbnailTimeKey: String

The frame number of an animation to use as a thumbnail image.

### Getting the Attachment Contents

var identifier: String

The unique identifier for the attachment.

var url: URL

The URL of the file for this attachment.

var type: String

The UTI type of the attachment.

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

### Notification content

Implementing communication notifications

Configure and display your app’s communication notifications by using intents.

protocol UNNotificationContentProviding

A protocol the system uses to provide context relevant to user notifications.

class UNNotificationActionIcon

An icon associated with an action.

class UNMutableNotificationContent

The editable content for a notification.

class UNNotificationContent

The uneditable content of a notification.

class UNNotificationSound

The sound played upon delivery of a notification.

struct UNNotificationSoundName

A string providing the name of a sound file.

