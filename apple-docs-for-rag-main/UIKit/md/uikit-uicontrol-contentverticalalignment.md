

- UIKit
- UIControl
-  contentVerticalAlignment 

Instance Property

# contentVerticalAlignment

The vertical alignment of content within the control’s bounds.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var contentVerticalAlignment: UIControl.ContentVerticalAlignment { get set }
```

## Parameters 

`contentAlignment`  

A constant that specifies the vertical alignment of text or images within the control. For a list of possible values, see UIControl.ContentVerticalAlignment.

## Discussion

For controls that contain configurable text or image content, use this property to align that content appropriately inside the control’s bounds. Not all control subclasses have content that can be aligned, and it’s the responsibility of the subclass to determine how to apply this value. The default value of this property is UIControl.ContentVerticalAlignment.top.

## See Also

### Specifying content alignment

enum ContentVerticalAlignment

Constants for specifying the vertical alignment of content (text and images) in a control.

var contentHorizontalAlignment: UIControl.ContentHorizontalAlignment

The horizontal alignment of content within the control’s bounds.

var effectiveContentHorizontalAlignment: UIControl.ContentHorizontalAlignment

The horizontal alignment currently in effect for the control.

enum ContentHorizontalAlignment

The horizontal alignment of content (text and images) within a control.

