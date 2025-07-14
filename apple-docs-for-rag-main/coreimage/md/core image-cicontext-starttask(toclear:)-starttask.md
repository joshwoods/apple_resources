

- Core Image
- CIContext
-  startTask(toClear:) 

Instance Method

# startTask(toClear:)

Fills the entire destination with black or clear depending on its alphaMode.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func startTask(toClear destination: CIRenderDestination) throws -> CIRenderTask
```

## Parameters 

`destination`  

The CIRenderDestination to clear.

`error`  

Pointer to an error object should the task fail.

## Return Value

The asynchronous CIRenderTask for clearing the destination.

## Discussion

If the destination's alphaMode is CIRenderDestinationAlphaMode.none, this command fills the entire destination with black `(0, 0, 0, 1)`.

If the destination's alphaMode is CIRenderDestinationAlphaMode.premultiplied or CIRenderDestinationAlphaMode.unpremultiplied, this command fills the entire destination with clear `(0, 0, 0, 0)`.

## See Also

### Customizing Render Destination

func prepareRender(CIImage, from: CGRect, to: CIRenderDestination, at: CGPoint)

An optional call to warm up a CIContext so that subsequent calls to render with the same arguments run more efficiently.

func startTask(toRender: CIImage, from: CGRect, to: CIRenderDestination, at: CGPoint) -> CIRenderTask

Renders a portion of an image to a point in the destination.

func startTask(toRender: CIImage, to: CIRenderDestination) -> CIRenderTask

Renders an image to a destination so that point (0, 0) of the image maps to point (0, 0) of the destination.

