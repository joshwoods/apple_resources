

- UIKit
- UITextSelectionRect
-  rect 

Instance Property

# rect

The rectangle that encloses the text selection rectangle’s text range.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var rect: CGRect { get }
```

## Discussion

The returned rectangle is in the coordinate system of the text input view that created the receiver.

