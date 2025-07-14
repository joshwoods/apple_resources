

- Messages
-  MSMessagesAppPresentationStyle 

Enumeration

# MSMessagesAppPresentationStyle

Presentation styles that describe your iMessage app’s appearance.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
enum MSMessagesAppPresentationStyle
```

## Topics

### Presentation Styles

case compact

The iMessage App is displayed inside the keyboard area.

case expanded

The iMessage App expands to fill most of the screen.

case transcript

The iMessage app is displayed in the Messages app’s transcript or input field.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Custom iMessage app interface

IceCreamBuilder: Building an iMessage Extension

Allow users to collaborate on the design of ice cream sundae stickers.

Creating a Sticker App with a Custom Layout

Expand on the Messages sticker app template to create an app with a customized user interface.

class MSMessagesAppViewController

The principal view controller for iMessage apps.

protocol MSMessagesAppTranscriptPresentation

A protocol that provides support for displaying live messages in the transcript of the Messages app.

