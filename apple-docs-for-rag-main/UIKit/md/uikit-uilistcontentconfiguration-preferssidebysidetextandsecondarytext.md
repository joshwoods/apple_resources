

- UIKit
- UIListContentConfiguration
-  prefersSideBySideTextAndSecondaryText 

Instance Property

# prefersSideBySideTextAndSecondaryText

A Boolean value that determines whether the configuration positions the text and secondary text side by side.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
var prefersSideBySideTextAndSecondaryText: Bool { get set }
```

## Discussion

When this value is true, the configuration positions the text and secondary text side by side if there’s sufficient space. Otherwise, the configuration stacks the text in a vertical layout.

## See Also

### Customizing layout

var axesPreservingSuperviewLayoutMargins: UIAxis

A Boolean value that determines whether the content view preserves the layout margins that it inherits from its superview on the horizontal or vertical axes.

var directionalLayoutMargins: NSDirectionalEdgeInsets

The margins between the content and the edges of the content view.

var imageToTextPadding: CGFloat

The padding between the image and text.

var textToSecondaryTextHorizontalPadding: CGFloat

The minimum horizontal padding between the text and secondary text.

var textToSecondaryTextVerticalPadding: CGFloat

The vertical padding between the text and secondary text.

