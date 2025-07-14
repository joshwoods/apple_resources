

- Messages
- MSMessagesAppViewController
-  didTransition(to:) 

Instance Method

# didTransition(to:)

Tells the view controller that the extension has transitioned to a new presentation style.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
@MainActor
func didTransition(to presentationStyle: MSMessagesAppPresentationStyle)
```

## Parameters 

`presentationStyle`  

The new presentation style. For a list of possible styles, see MSMessagesAppPresentationStyle.

## Discussion

Override this method to respond after the extension’s user interface has transitioned to a new presentation style. The user can switch between styles by tapping the collapse and expand buttons in the Messages app. You can also programmatically trigger a transition by calling requestPresentationStyle(_:).

The system doesn’t call this method on a view controller that is presenting a live view in the transcript or input field—in other words, when the view controller’s presentationStyle property is set to the MSMessagesAppPresentationStyle.transcript value.

## See Also

### Working with Presentation Styles and Contexts

var presentationStyle: MSMessagesAppPresentationStyle

The extension’s current presentation style.

func requestPresentationStyle(MSMessagesAppPresentationStyle)

Asks the extension’s user interface to transition to the provided style.

func willTransition(to: MSMessagesAppPresentationStyle)

Tells the view controller that the extension is about to transition to a new presentation style.

enum MSMessagesAppPresentationStyle

Presentation styles that describe your iMessage app’s appearance.

var presentationContext: MSMessagesAppPresentationContext

The context describing where your iMessage app is presented.

enum MSMessagesAppPresentationContext

Presentation contexts describing where your iMessage app appears.

