

- UIKit
- UIListContentConfiguration
-  textToSecondaryTextVerticalPadding 

Instance Property

# textToSecondaryTextVerticalPadding

The vertical padding between the text and secondary text.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
var textToSecondaryTextVerticalPadding: CGFloat { get set }
```

## Discussion

This value only applies when there’s both text and secondary text, and they’re in a stacked vertical layout.

## See Also

### Customizing layout

var axesPreservingSuperviewLayoutMargins: UIAxis

A Boolean value that determines whether the content view preserves the layout margins that it inherits from its superview on the horizontal or vertical axes.

var directionalLayoutMargins: NSDirectionalEdgeInsets

The margins between the content and the edges of the content view.

var prefersSideBySideTextAndSecondaryText: Bool

A Boolean value that determines whether the configuration positions the text and secondary text side by side.

var imageToTextPadding: CGFloat

The padding between the image and text.

var textToSecondaryTextHorizontalPadding: CGFloat

The minimum horizontal padding between the text and secondary text.

