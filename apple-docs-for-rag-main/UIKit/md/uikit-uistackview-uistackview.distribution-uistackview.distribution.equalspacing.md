

- UIKit
- UIStackView
- UIStackView.Distribution
-  UIStackView.Distribution.equalSpacing 

Case

# UIStackView.Distribution.equalSpacing

A layout where the stack view positions its arranged views so that they fill the available space along the stack view’s axis.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
case equalSpacing
```

## Discussion

When the arranged views don’t fill the stack view, it pads the spacing between the views evenly. If the arranged views don’t fit within the stack view, it shrinks the views according to their compression resistance priority. If there’s any ambiguity, the stack view shrinks the views based on their index in the arrangedSubviews array.

The following image shows an example of a horizontal stack view that uses the UIStackView.Distribution.equalSpacing distribution.

## See Also

### Constants

case fill

A layout where the stack view resizes its arranged views so that they fill the available space along the stack view’s axis.

case fillEqually

A layout where the stack view resizes its arranged views so that they fill the available space along the stack view’s axis.

case fillProportionally

A layout where the stack view resizes its arranged views so that they fill the available space along the stack view’s axis.

case equalCentering

A layout that attempts to position the arranged views with equal center-to-center spacing along the stack view’s axis, while maintaining the spacing property’s distance between views.

