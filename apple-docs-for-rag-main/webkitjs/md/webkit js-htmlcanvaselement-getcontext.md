

- WebKit JS
- HTMLCanvasElement
-  getContext 

Instance Method

# getContext

Returns the drawing context for the canvas.

Safari Desktop 3.0+Safari Mobile 1.0+

``` source
RenderingContext? getContext(
    DOMString contextId, 
    any ... arguments
);
```

## Parameters 

`contextId`  

The identifier for the context. Currently, only the identifier `"2d"` is supported.

## Return Value

The context object. Currently, always a `CanvasRenderingContext2D` object.

## Discussion

Use the `getContext` method to obtain a drawing context for the canvas. All drawing on the canvas is done using the methods and properties of the context.

