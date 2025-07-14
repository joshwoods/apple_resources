

- UIKit
- UIGraphicsRendererContext
-  format 

Instance Property

# format

The format used to create the associated graphics renderer.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
var format: UIGraphicsRendererFormat { get }
```

## Discussion

If you specified a format object when you initialized the current renderer (UIGraphicsRenderer) object, then this property provides access to that object. Otherwise, a default format object was created for you using the renderer initialization parameters, tuned to the current device.

## See Also

### Getting the drawing context

var cgContext: CGContext

The underlying Core Graphics context.

