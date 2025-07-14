

- UIKit
- UIStackView
- UIStackView.Distribution
-  UIStackView.Distribution.equalCentering 

Case

# UIStackView.Distribution.equalCentering

A layout that attempts to position the arranged views with equal center-to-center spacing along the stack view’s axis, while maintaining the spacing property’s distance between views.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
case equalCentering
```

## Discussion

If the arranged views don’t fit within the stack view, it shrinks the spacing until it reaches the minimum spacing defined by its spacing property. If the views still don’t fit, the stack view shrinks the arranged views according to their compression resistance priority. If there’s any ambiguity, the stack view shrinks the views based on their index in the arrangedSubviews array.

The following image shows an example of a horizontal stack view that uses the UIStackView.Distribution.equalSpacing distribution.

Note

The stack view maintains the intrinsic content size of its arranged views at the expense of the center-to-center spacing. Similarly, it maintains the minimum spacing between views at the expense of the view’s intrinsic content size.

## See Also

### Constants

case fill

A layout where the stack view resizes its arranged views so that they fill the available space along the stack view’s axis.

case fillEqually

A layout where the stack view resizes its arranged views so that they fill the available space along the stack view’s axis.

case fillProportionally

A layout where the stack view resizes its arranged views so that they fill the available space along the stack view’s axis.

case equalSpacing

A layout where the stack view positions its arranged views so that they fill the available space along the stack view’s axis.

