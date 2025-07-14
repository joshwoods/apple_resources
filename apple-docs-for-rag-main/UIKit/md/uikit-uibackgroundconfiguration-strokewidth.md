

- UIKit
- UIBackgroundConfiguration
-  strokeWidth 

Instance Property

# strokeWidth

The width of the stroke.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
var strokeWidth: CGFloat { get set }
```

## Discussion

The default value is `0.0`.

## See Also

### Customizing the background

var customView: UIView?

A custom view for the background.

var cornerRadius: CGFloat

The preferred corner radius, using a continuous corner curve, for the background and stroke.

var backgroundInsets: NSDirectionalEdgeInsets

The insets (or outsets, if negative) for the background and stroke, relative to the edges of the containing view.

var edgesAddingLayoutMarginsToBackgroundInsets: NSDirectionalRectEdge

The edges on which the configuration adds the containing view’s layout margins to the background insets.

var backgroundColor: UIColor?

The color of the background.

var backgroundColorTransformer: UIConfigurationColorTransformer?

The color transformer for resolving the background color.

func resolvedBackgroundColor(for: UIColor) -> UIColor

Generates the resolved background color for the specified tint color, using the background color and color transformer.

var visualEffect: UIVisualEffect?

The visual effect that the configuration applies to the background.

var strokeColor: UIColor?

The color of the stroke.

var strokeColorTransformer: UIConfigurationColorTransformer?

The color transformer for resolving the stroke color.

func resolvedStrokeColor(for: UIColor) -> UIColor

Generates the resolved stroke color for the specified tint color, using the stroke color and color transformer.

var strokeOutset: CGFloat

The outset (or inset, if negative) for the stroke.

var image: UIImage?

The image displayed in the view’s background.

var imageContentMode: UIView.ContentMode

A property that determines the layout of a background image in a view when its bounds change.

