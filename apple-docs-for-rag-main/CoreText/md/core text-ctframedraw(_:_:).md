

- Core Text
-  CTFrameDraw(\_:\_:) 

Function

# CTFrameDraw(\_:\_:)

Draws an entire frame into a context.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFrameDraw(
    _ frame: CTFrame,
    _ context: CGContext
)
```

## Parameters 

`frame`  

The frame to draw.

`context`  

The context in which to draw the frame.

## Discussion

If both the frame and the context are valid, the frame is drawn in the context. This call can leave the context in any state and does not flush it after the draw operation.

