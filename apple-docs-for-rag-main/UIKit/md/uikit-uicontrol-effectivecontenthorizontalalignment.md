

- UIKit
- UIControl
-  effectiveContentHorizontalAlignment 

Instance Property

# effectiveContentHorizontalAlignment

The horizontal alignment currently in effect for the control.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var effectiveContentHorizontalAlignment: UIControl.ContentHorizontalAlignment { get }
```

## Discussion

This property always contains the value UIControl.ContentHorizontalAlignment.left or UIControl.ContentHorizontalAlignment.right, even when the actual horizontal alignment is UIControl.ContentHorizontalAlignment.leading or UIControl.ContentHorizontalAlignment.trailing.

## See Also

### Specifying content alignment

var contentVerticalAlignment: UIControl.ContentVerticalAlignment

The vertical alignment of content within the control’s bounds.

enum ContentVerticalAlignment

Constants for specifying the vertical alignment of content (text and images) in a control.

var contentHorizontalAlignment: UIControl.ContentHorizontalAlignment

The horizontal alignment of content within the control’s bounds.

enum ContentHorizontalAlignment

The horizontal alignment of content (text and images) within a control.

