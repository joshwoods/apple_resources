

- Messages
- MSMessagesAppViewController
-  willTransition(to:) 

Instance Method

# willTransition(to:)

Tells the view controller that the extension is about to transition to a new presentation style.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
@MainActor
func willTransition(to presentationStyle: MSMessagesAppPresentationStyle)
```

## Parameters 

`presentationStyle`  

The new presentation style. For a list of possible styles, see MSMessagesAppPresentationStyle.

## Discussion

Override this method to update your extension’s layout while the extension is transitioning between the MSMessagesAppPresentationStyle.compact and MSMessagesAppPresentationStyle.expanded styles. The user can switch between styles by tapping the collapse and expand buttons in the Messages app. You can also programmatically trigger a transition by calling requestPresentationStyle(_:).

The system doesn’t call this method on a view controller that is presenting a live view in the transcript or input field—in other words, when the view controller’s presentationStyle property is set to the MSMessagesAppPresentationStyle.transcript value.

Note

Because the keyboard is not available in the MSMessagesAppPresentationStyle.compact style, adding text fields or text views to your compact layout is not recommended.

## See Also

### Working with Presentation Styles and Contexts

var presentationStyle: MSMessagesAppPresentationStyle

The extension’s current presentation style.

func requestPresentationStyle(MSMessagesAppPresentationStyle)

Asks the extension’s user interface to transition to the provided style.

func didTransition(to: MSMessagesAppPresentationStyle)

Tells the view controller that the extension has transitioned to a new presentation style.

enum MSMessagesAppPresentationStyle

Presentation styles that describe your iMessage app’s appearance.

var presentationContext: MSMessagesAppPresentationContext

The context describing where your iMessage app is presented.

enum MSMessagesAppPresentationContext

Presentation contexts describing where your iMessage app appears.

