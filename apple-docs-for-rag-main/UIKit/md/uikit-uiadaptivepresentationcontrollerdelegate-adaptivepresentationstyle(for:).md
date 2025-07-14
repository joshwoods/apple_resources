

- UIKit
- UIAdaptivePresentationControllerDelegate
-  adaptivePresentationStyle(for:) 

Instance Method

# adaptivePresentationStyle(for:)

Asks the delegate for the new presentation style to use.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func adaptivePresentationStyle(for controller: UIPresentationController) -> UIModalPresentationStyle
```

## Parameters 

`controller`  

The presentation controller that is managing the size change. Use this object to retrieve the view controllers involved in the presentation.

## Return Value

The new presentation style, which must be UIModalPresentationStyle.fullScreen, UIModalPresentationStyle.overFullScreen, or UIModalPresentationStyle.none.

## Discussion

In iOS 8.3 and later, use the adaptivePresentationStyle(for:traitCollection:) method to handle all trait changes instead of this method. If you do not implement that method, you can use this method to change the presentation style when transitioning to a horizontally compact environment.

If you do not implement this method or if you return an invalid style, the current presentation controller returns its preferred default style.

## See Also

### Adapting the presentation style

func adaptivePresentationStyle(for: UIPresentationController, traitCollection: UITraitCollection) -> UIModalPresentationStyle

Asks the delegate for the presentation style to use when the specified set of traits are active.

