

- UIKit
- UISheetPresentationController
-  largestUndimmedDetentIdentifier 

Instance Property

# largestUndimmedDetentIdentifier

The largest detent that doesn’t dim the view underneath the sheet.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
@MainActor
var largestUndimmedDetentIdentifier: UISheetPresentationController.Detent.Identifier? { get set }
```

## Discussion

The default value is `nil`, which means the system adds a noninteractive dimming view underneath the sheet at all detents. Set this property to only add the dimming view at detents larger than the detent you specify. For example, set this property to medium to add the dimming view at the large detent.

Without a dimming view, the undimmed area around the sheet responds to user interaction, allowing for a nonmodal experience. You can use this behavior for sheets with interactive content underneath them.

## See Also

### Managing user interaction

var prefersScrollingExpandsWhenScrolledToEdge: Bool

A Boolean value that determines whether scrolling expands the sheet to a larger detent.

