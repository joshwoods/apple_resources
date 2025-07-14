

- UIKit
- UIAdaptivePresentationControllerDelegate
-  adaptivePresentationStyle(for:traitCollection:) 

Instance Method

# adaptivePresentationStyle(for:traitCollection:)

Asks the delegate for the presentation style to use when the specified set of traits are active.

iOS 8.3+iPadOS 8.3+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func adaptivePresentationStyle(
    for controller: UIPresentationController,
    traitCollection: UITraitCollection
) -> UIModalPresentationStyle
```

## Parameters 

`controller`  

The presentation controller that is managing the size change. Use this object to retrieve the view controllers involved in the presentation.

`traitCollection`  

The traits representing the target environment.

## Return Value

The new presentation style, which must be UIModalPresentationStyle.fullScreen, UIModalPresentationStyle.overFullScreen, UIModalPresentationStyle.formSheet, or UIModalPresentationStyle.none.

## Discussion

The presentation controller calls this method when the traits of the current environment are about to change. Your implementation of this method can return the preferred presentation style to use for the specified traits. If you do not return one of the allowed styles, the presentation controller uses its preferred default style.

If you do not implement this method in your delegate, UIKit calls the adaptivePresentationStyle(for:) method instead.

## See Also

### Adapting the presentation style

func adaptivePresentationStyle(for: UIPresentationController) -> UIModalPresentationStyle

Asks the delegate for the new presentation style to use.

