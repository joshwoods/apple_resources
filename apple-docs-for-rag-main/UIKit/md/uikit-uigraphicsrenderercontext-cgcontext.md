

- UIKit
- UIGraphicsRendererContext
-  cgContext 

Instance Property

# cgContext

The underlying Core Graphics context.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
var cgContext: CGContext { get }
```

## Discussion

Use this property to gain access to the underlying Core Graphics context when you need more drawing functionality than is offered by UIKit and `UIGraphicsRendererContext`.

For an example of how and when to use the Core Graphics context in an image renderer, see Using Core Graphics rendering functions in UIGraphicsImageRenderer.

## See Also

### Getting the drawing context

var format: UIGraphicsRendererFormat

The format used to create the associated graphics renderer.

