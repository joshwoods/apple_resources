

- UIKit
- UIKeyboardLayoutGuide
-  usesBottomSafeArea 

Instance Property

# usesBottomSafeArea

A Boolean value that indicates whether the layout guide uses the view’s safe area layout guide.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
var usesBottomSafeArea: Bool { get set }
```

## Discussion

Defaults to true, indicating that the layout guide ties to the bottomAnchor of the view’s safeAreaLayoutGuide.

Set to false to tie the layout guide to the bottomAnchor of the view instead.

