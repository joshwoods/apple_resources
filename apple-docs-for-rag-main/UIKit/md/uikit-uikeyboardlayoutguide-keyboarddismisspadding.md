

- UIKit
- UIKeyboardLayoutGuide
-  keyboardDismissPadding 

Instance Property

# keyboardDismissPadding

A value that adds padding above the keyboard to increase the size of the touch area for the scrolling dismissal gesture.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
var keyboardDismissPadding: CGFloat { get set }
```

## Discussion

Defaults to `0`. The system treats negative values as `0`.

