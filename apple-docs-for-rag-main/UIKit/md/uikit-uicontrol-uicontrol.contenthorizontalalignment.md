

- UIKit
- UIControl
-  UIControl.ContentHorizontalAlignment 

Enumeration

# UIControl.ContentHorizontalAlignment

The horizontal alignment of content (text and images) within a control.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum ContentHorizontalAlignment
```

## Overview

You use these constants as the value of the contentHorizontalAlignment property.

## Topics

### Constants

case center

Aligns the content horizontally in the center of the control.

case left

Aligns the content horizontally from the left of the control (the default).

case right

Aligns the content horizontally from the right of the control.

case fill

Aligns the content horizontally to fill the content rectangles; text may wrap and images may be stretched.

case leading

Aligns the content horizontally from the leading edge of the control.

case trailing

Aligns the content horizontally from the trailing edge of the control.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Specifying content alignment

var contentVerticalAlignment: UIControl.ContentVerticalAlignment

The vertical alignment of content within the control’s bounds.

enum ContentVerticalAlignment

Constants for specifying the vertical alignment of content (text and images) in a control.

var contentHorizontalAlignment: UIControl.ContentHorizontalAlignment

The horizontal alignment of content within the control’s bounds.

var effectiveContentHorizontalAlignment: UIControl.ContentHorizontalAlignment

The horizontal alignment currently in effect for the control.

