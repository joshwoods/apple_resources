

- Messages
- MSMessagesAppViewController
-  requestPresentationStyle(\_:) 

Instance Method

# requestPresentationStyle(\_:)

Asks the extension’s user interface to transition to the provided style.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
@MainActor
func requestPresentationStyle(_ presentationStyle: MSMessagesAppPresentationStyle)
```

## Parameters 

`presentationStyle`  

The desired presentation style. For a list of possible styles, see MSMessagesAppPresentationStyle.

## Discussion

Use this method when you need to change the extension’s presentation style. Keep in mind that the user should have ultimate control over the extension’s presentation style. If the user chooses to change the presentation style, you want to respect that choice.

Important

You cannot pass the MSMessagesAppPresentationStyle.transcript presentation style to this method.

If you call this method on a view controller with a MSMessagesAppPresentationStyle.transcript presentation style (which is a controller that’s presenting an interactive view in the transcript), the system creates a new instance of the view controller and displays it using the provided presentation style.

## See Also

### Working with Presentation Styles and Contexts

var presentationStyle: MSMessagesAppPresentationStyle

The extension’s current presentation style.

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

