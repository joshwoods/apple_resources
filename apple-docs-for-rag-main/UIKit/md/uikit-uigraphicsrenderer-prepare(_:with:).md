

- UIKit
- UIGraphicsRenderer
-  prepare(\_:with:) 

Type Method

# prepare(\_:with:)

Applies the configuration specified in the renderer context to the Core Graphics context.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
class func prepare(
    _ context: CGContext,
    with rendererContext: UIGraphicsRendererContext
)
```

## Parameters 

`context`  

The Core Graphics context that the graphics renderer performs drawing actions on.

`rendererContext`  

The renderer context object that is provided to the runDrawingActions(_:completionActions:) method. This object is of the type returned by the rendererContextClass() static method.

## Discussion

The graphics renderer calls this method when the runDrawingActions(_:completionActions:) method is invoked. Override this method in a subclass to configure the underlying Core Graphics context before the renderer begins renderering.

Core Graphics contexts are reused for repeated calls to the runDrawingActions(_:completionActions:) method. Therefore, be sure to clean up the context to make it ready for reuse.

## See Also

### Managing graphics contexts

class func context(with: UIGraphicsRendererFormat) -> CGContext?

Creates a Core Graphics context configured according to the supplied format object.

class func rendererContextClass() -> AnyClass

Specifies the drawing context class used by this graphics renderer.

