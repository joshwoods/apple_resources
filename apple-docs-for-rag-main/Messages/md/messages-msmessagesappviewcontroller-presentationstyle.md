

- Messages
- MSMessagesAppViewController
-  presentationStyle 

Instance Property

# presentationStyle

The extension’s current presentation style.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
@MainActor
var presentationStyle: MSMessagesAppPresentationStyle { get }
```

## Discussion

The presentation style defines how the extension appears in the Messages app. The property’s value is set by the following actions:

- The user selects the extension in the app drawer: The Messages app launches the extension using the MSMessagesAppPresentationStyle.compact style.

- The user selects a message in the transcript that represents one of the extension’s MSMessage objects: The Messages app launches the extension using the MSMessagesAppPresentationStyle.expanded style.

- The user taps the collapse and expand buttons while the extension is running: The Messages app changes the current presentation style.

- You programmatically set the presentation style by calling the requestPresentationStyle(_:) method.

## See Also

### Working with Presentation Styles and Contexts

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

enum MSMessagesAppPresentationContext

Presentation contexts describing where your iMessage app appears.

