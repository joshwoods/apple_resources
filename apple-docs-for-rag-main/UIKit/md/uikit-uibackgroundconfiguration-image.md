

- UIKit
- UIBackgroundConfiguration
-  image 

Instance Property

# image

The image displayed in the view’s background.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
var image: UIImage? { get set }
```

## Discussion

This property contains the image displayed in the view’s background. If this property is set to `nil`, the view displays no background image.

Changing the image in this property doesn’t change the size of the view automatically. You can use the background configuration’s imageContentMode to specify how to lay out the image when its size differs from the size in the view’s bounds.

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

var strokeWidth: CGFloat

The width of the stroke.

var strokeOutset: CGFloat

The outset (or inset, if negative) for the stroke.

var imageContentMode: UIView.ContentMode

A property that determines the layout of a background image in a view when its bounds change.

