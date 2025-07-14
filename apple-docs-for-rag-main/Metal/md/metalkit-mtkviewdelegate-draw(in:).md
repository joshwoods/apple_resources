

- MetalKit
- MTKViewDelegate
-  draw(in:) 

Instance Method

# draw(in:)

Draws the view’s contents.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func draw(in view: MTKView)
```

**Required**

## Parameters 

`view`  

The view requesting that its contents be redrawn.

## Discussion

This method is called on the delegate when it is asked to render into the view.

