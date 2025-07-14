

- Core Image
- CIContext
-  startTask(toRender:from:to:at:) 

Instance Method

# startTask(toRender:from:to:at:)

Renders a portion of an image to a point in the destination.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func startTask(
    toRender image: CIImage,
    from fromRect: CGRect,
    to destination: CIRenderDestination,
    at atPoint: CGPoint
) throws -> CIRenderTask
```

## Parameters 

`image`  

A CIImage to render.

`fromRect`  

The part of the image to render, as if cropped.

`destination`  

A CIRenderDestination into which to render the image.

`atPoint`  

An origin point in the destination at which to place the image.

## Return Value

An asynchronous CIRenderTask to render the image to the specified destination.

## Discussion

This method crops the image to the specified rectangle and renders the result at the indicated origin point. If the image’s extent property and `fromRect` argument values are infinite, this call renders the image’s (0, 0) point starting from the origin `atPoint`.

You must use an MTLTexture-backed CIContext to support an `MTLTexture`-backed CIRenderDestination. Similarly, you must use `GLContext`-backed CIContext to support a `GLTexture`-backed CIRenderDestination.

This call returns as soon as it enqueues all work required to render the image on the context’s device. In many situations, after issuing a render, you may need to wait for it to complete. In these cases, use the returned CIRenderTask as follows:

let renderTask = try context.startTask(toRender: image, from: fromRect, to: destination, at: point)

let renderInfo = try renderTask.waitUntilCompleted()

## See Also

### Customizing Render Destination

func prepareRender(CIImage, from: CGRect, to: CIRenderDestination, at: CGPoint)

An optional call to warm up a CIContext so that subsequent calls to render with the same arguments run more efficiently.

func startTask(toClear: CIRenderDestination) -> CIRenderTask

Fills the entire destination with black or clear depending on its alphaMode.

func startTask(toRender: CIImage, to: CIRenderDestination) -> CIRenderTask

Renders an image to a destination so that point (0, 0) of the image maps to point (0, 0) of the destination.

