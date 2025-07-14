

- UIKit
- UIControl
-  UIControl.ContentVerticalAlignment 

Enumeration

# UIControl.ContentVerticalAlignment

Constants for specifying the vertical alignment of content (text and images) in a control.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum ContentVerticalAlignment
```

## Overview

You use these constants as the value of the contentVerticalAlignment property.

## Topics

### Constants

case center

Aligns the content vertically in the center of the control.

case top

Aligns the content vertically at the top in the control (the default).

case bottom

Aligns the content vertically at the bottom in the control.

case fill

Aligns the content vertically to fill the content rectangle; images may be stretched.

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

var contentHorizontalAlignment: UIControl.ContentHorizontalAlignment

The horizontal alignment of content within the control’s bounds.

var effectiveContentHorizontalAlignment: UIControl.ContentHorizontalAlignment

The horizontal alignment currently in effect for the control.

enum ContentHorizontalAlignment

The horizontal alignment of content (text and images) within a control.

