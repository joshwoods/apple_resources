

- UIKit
- UIGraphicsRenderer
-  runDrawingActions(\_:completionActions:) 

Instance Method

# runDrawingActions(\_:completionActions:)

Performs drawing actions on a Core Graphics context that the renderer prepares.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
func runDrawingActions(
    _ drawingActions: (UIGraphicsRendererContext) -> Void,
    completionActions: ((UIGraphicsRendererContext) -> Void)? = nil
) throws
```

## Parameters 

`drawingActions`  

A UIGraphicsDrawingActions block that represents a set of drawing instructions that the renderer applies to the Core Graphics context.

`completionActions`  

A UIGraphicsDrawingActions block that the renderer calls after executing the `drawingActions` block.

## Discussion

This method invokes the `drawingActions` block in a Core Graphics context. This context was created by the context(with:) method, captured in an instance of the class returned by the rendererContextClass() method, and prepared by the prepare(_:with:) method.

Do not override this method. Instead, consider invoking it from a utility method in your subclass, as the UIGraphicsImageRenderer and UIGraphicsPDFRenderer classes do.

## See Also

### Running the drawing actions

typealias UIGraphicsDrawingActions

A closure that executes a set of drawing instructions that the renderer applies to the Core Graphics context.

