

- Messages
-  MSMessagesAppPresentationContext 

Enumeration

# MSMessagesAppPresentationContext

Presentation contexts describing where your iMessage app appears.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
enum MSMessagesAppPresentationContext
```

## Topics

### Presentation Contexts

case media

A constant that indicates the iMessage app appears inside the Stickers app throughout iOS including in Messages, FaceTime, the emoji keyboard, and Markup.

case messages

A constant that indicates the iMessage app appears in Messages in the list of iMessage apps that appears when you press the plus button.

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

### Working with Presentation Styles and Contexts

var presentationStyle: MSMessagesAppPresentationStyle

The extension’s current presentation style.

func requestPresentationStyle(MSMessagesAppPresentationStyle)

Asks the extension’s user interface to transition to the provided style.

func willTransition(to: MSMessagesAppPresentationStyle)

Tells the view controller that the extension is about to transition to a new presentation style.

func didTransition(to: MSMessagesAppPresentationStyle)

Tells the view controller that the extension has transitioned to a new presentation style.

enum MSMessagesAppPresentationStyle

Presentation styles that describe your iMessage app’s appearance.

var presentationContext: MSMessagesAppPresentationContext

The context describing where your iMessage app is presented.

