

- UIKit
- UIListContentConfiguration
-  directionalLayoutMargins 

Instance Property

# directionalLayoutMargins

The margins between the content and the edges of the content view.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
var directionalLayoutMargins: NSDirectionalEdgeInsets { get set }
```

## Discussion

When you preserve superview layout margins on one or both axes, this value specifies the minimum margins. The inherited margins may be larger.

By default, the content view preserves the layout margins of its superview on both axes. You can customize this behavior by changing axesPreservingSuperviewLayoutMargins.

## See Also

### Customizing layout

var axesPreservingSuperviewLayoutMargins: UIAxis

A Boolean value that determines whether the content view preserves the layout margins that it inherits from its superview on the horizontal or vertical axes.

var prefersSideBySideTextAndSecondaryText: Bool

A Boolean value that determines whether the configuration positions the text and secondary text side by side.

var imageToTextPadding: CGFloat

The padding between the image and text.

var textToSecondaryTextHorizontalPadding: CGFloat

The minimum horizontal padding between the text and secondary text.

var textToSecondaryTextVerticalPadding: CGFloat

The vertical padding between the text and secondary text.

