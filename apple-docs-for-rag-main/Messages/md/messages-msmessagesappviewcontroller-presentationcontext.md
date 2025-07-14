

- Messages
- MSMessagesAppViewController
-  presentationContext 

Instance Property

# presentationContext

The context describing where your iMessage app is presented.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
@MainActor
var presentationContext: MSMessagesAppPresentationContext { get }
```

## Mentioned in 

Adding Sticker packs and iMessage apps to the system Stickers app, Messages camera, and FaceTime

## Discussion

By default, the system only displays iMessage apps in the MSMessagesAppPresentationContext.messages context (the iMessage app only appears inside the Messages app). iMessage apps in the media context have additional limitations and design considerations.

You can control the supported contexts by adding the `MSSupportedPresentationContexts` key to the iMessage app extension’s `Info.plist` file. For example, presentationContext enables the iMessage app in effects in Messages and FaceTime.

```
```

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

enum MSMessagesAppPresentationContext

Presentation contexts describing where your iMessage app appears.

