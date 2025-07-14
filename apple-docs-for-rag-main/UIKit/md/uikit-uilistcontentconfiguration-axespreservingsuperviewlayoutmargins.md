

- UIKit
- UIListContentConfiguration
-  axesPreservingSuperviewLayoutMargins 

Instance Property

# axesPreservingSuperviewLayoutMargins

A Boolean value that determines whether the content view preserves the layout margins that it inherits from its superview on the horizontal or vertical axes.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
var axesPreservingSuperviewLayoutMargins: UIAxis { get set }
```

## Discussion

By default, the content view preserves the layout margins of its superview on both axes.

## See Also

### Customizing layout

var directionalLayoutMargins: NSDirectionalEdgeInsets

The margins between the content and the edges of the content view.

var prefersSideBySideTextAndSecondaryText: Bool

A Boolean value that determines whether the configuration positions the text and secondary text side by side.

var imageToTextPadding: CGFloat

The padding between the image and text.

var textToSecondaryTextHorizontalPadding: CGFloat

The minimum horizontal padding between the text and secondary text.

var textToSecondaryTextVerticalPadding: CGFloat

The vertical padding between the text and secondary text.

