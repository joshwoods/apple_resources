

- UIKit
- UISheetPresentationController
-  prefersScrollingExpandsWhenScrolledToEdge 

Instance Property

# prefersScrollingExpandsWhenScrolledToEdge

A Boolean value that determines whether scrolling expands the sheet to a larger detent.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
@MainActor
var prefersScrollingExpandsWhenScrolledToEdge: Bool { get set }
```

## Discussion

The default value is true, which means if the sheet can expand to a larger detent than selectedDetentIdentifier, scrolling up in the sheet increases its detent instead of scrolling the sheet’s content. After the sheet reaches its largest detent, scrolling begins.

Set this value to false if you want to avoid letting a scroll gesture expand the sheet. For example, you can set this value on a nonmodal sheet to avoid obscuring the content underneath the sheet.

## See Also

### Managing user interaction

var largestUndimmedDetentIdentifier: UISheetPresentationController.Detent.Identifier?

The largest detent that doesn’t dim the view underneath the sheet.

