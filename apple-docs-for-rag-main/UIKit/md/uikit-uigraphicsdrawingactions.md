

- UIKit
-  UIGraphicsDrawingActions 

Type Alias

# UIGraphicsDrawingActions

A closure that executes a set of drawing instructions that the renderer applies to the Core Graphics context.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
typealias UIGraphicsDrawingActions = (UIGraphicsRendererContext) -> Void
```

## Discussion

UIGraphicsDrawingActions defines a block type that takes a UIGraphicsRendererContext object as an argument and has no return value.

You provide a block of this type as an argument to the graphics drawing methods on UIGraphicsRenderer. Your block should use the provided renderer context to perform the drawing operations you want the renderer to execute.

## See Also

### Related Documentation

typealias DrawingActions

A closure for drawing an image.

typealias DrawingActions

A closure for drawing PDF content.

### Running the drawing actions

func runDrawingActions((UIGraphicsRendererContext) -> Void, completionActions: ((UIGraphicsRendererContext) -> Void)?) throws

Performs drawing actions on a Core Graphics context that the renderer prepares.

