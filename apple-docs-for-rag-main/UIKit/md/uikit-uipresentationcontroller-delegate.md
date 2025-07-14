

- UIKit
- UIPresentationController
-  delegate 

Instance Property

# delegate

The delegate object for managing adaptive presentations.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
weak var delegate: (any UIAdaptivePresentationControllerDelegate)? { get set }
```

## Discussion

When the app’s size changes, the presentation controller works with this delegate object to determine an appropriate response. View controllers presented using the UIModalPresentationStyle.formSheet, UIModalPresentationStyle.popover, or UIModalPresentationStyle.custom style must change to use one of the full-screen presentation styles instead. The delegate can also opt to change the presented view controller entirely.

The object you assign to this property must conform to the UIAdaptivePresentationControllerDelegate protocol.

## See Also

### Adapting your presentations dynamically

protocol UIAdaptivePresentationControllerDelegate

A set of methods that, in conjunction with a presentation controller, determine how to respond to trait changes in your app.

