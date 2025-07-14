

- UIKit
- UIGraphicsRenderer
-  allowsImageOutput 

Instance Property

# allowsImageOutput

A Boolean value specifying whether the renderer can create output images.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
var allowsImageOutput: Bool { get }
```

## Discussion

If true, this renderer can be used to generate CGImage objects.

## See Also

### Configuring the renderer

var format: UIGraphicsRendererFormat

The format used to create the graphics renderer.

