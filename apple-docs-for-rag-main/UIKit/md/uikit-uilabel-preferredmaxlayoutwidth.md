

- UIKit
- UILabel
-  preferredMaxLayoutWidth 

Instance Property

# preferredMaxLayoutWidth

The preferred maximum width, in points, for a multiline label.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var preferredMaxLayoutWidth: CGFloat { get set }
```

## Discussion

This property affects the size of the label when the system applies layout constraints to it. During layout, if the text extends beyond the width specified by this property, the additional text flows to one or more new lines, increasing the height of the label.

