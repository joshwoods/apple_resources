

- Messages
-  MSMessageTemplateLayout 

Class

# MSMessageTemplateLayout

A template-based layout for custom messages.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
class MSMessageTemplateLayout
```

## Overview

The MSMessageTemplateLayout describes how an MSMessage object is presented in the transcript. The message template includes the Message extension’s icon, an image, video, or audio file, and a number of text elements (title, subtitle, caption, subcaption, trailing caption, and trailing subcaption). These elements are laid out as shown in Figure 1.

To use the template:

1.  Instantiate a new `MSMessageTemplateLayout` object.

2.  Assign values to the properties representing the desired visual elements. You can leave unwanted elements set to `nil`. The system sizes the message balloon to fit the provided content.

3.  Assign the `MSMessageTemplateLayout` object to the MSMessage object’s layout property.

Do not subclass the `MSMessageTemplateLayout` class.

## Topics

### Assigning Visual Elements

var image: UIImage?

An image used to represent the message in the transcript.

var mediaFileURL: URL?

A media file used to represent the message in the transcript.

var imageTitle: String?

The title for the image or media file.

var imageSubtitle: String?

The subtitle for the image or media file.

var caption: String?

A left-aligned caption for the message bubble.

var subcaption: String?

A left-aligned subcaption for the message bubble.

var trailingCaption: String?

A right-aligned caption for the message bubble.

var trailingSubcaption: String?

A right-aligned subcaption for the message bubble.

## Relationships

### Inherits From

- MSMessageLayout

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Interactive messages

class MSMessage

A custom message object.

class MSSession

A session object used to create and update messages.

class MSMessageLayout

An abstract base class that defines the appearance of MSMessage objects in the conversation transcript.

class MSMessageLiveLayout

A layout that provides a custom, interactive view inside the transcript.

