

- Core Image
- CIContext
-  startTask(toRender:to:) 

Instance Method

# startTask(toRender:to:)

Renders an image to a destination so that point (0, 0) of the image maps to point (0, 0) of the destination.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func startTask(
    toRender image: CIImage,
    to destination: CIRenderDestination
) throws -> CIRenderTask
```

## Parameters 

`image`  

CIImage to prepare to render.

`destination`  

The CIRenderDestination to which to render.

`error`  

Pointer to an error should the render task creation fail.

## Return Value

The asynchronous CIRenderTask to render the image to the specified destination.

## See Also

### Customizing Render Destination

func prepareRender(CIImage, from: CGRect, to: CIRenderDestination, at: CGPoint)

An optional call to warm up a CIContext so that subsequent calls to render with the same arguments run more efficiently.

func startTask(toClear: CIRenderDestination) -> CIRenderTask

Fills the entire destination with black or clear depending on its alphaMode.

func startTask(toRender: CIImage, from: CGRect, to: CIRenderDestination, at: CGPoint) -> CIRenderTask

Renders a portion of an image to a point in the destination.

