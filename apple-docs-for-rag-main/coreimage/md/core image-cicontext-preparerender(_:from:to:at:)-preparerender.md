

- Core Image
- CIContext
-  prepareRender(\_:from:to:at:) 

Instance Method

# prepareRender(\_:from:to:at:)

An optional call to warm up a CIContext so that subsequent calls to render with the same arguments run more efficiently.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func prepareRender(
    _ image: CIImage,
    from fromRect: CGRect,
    to destination: CIRenderDestination,
    at atPoint: CGPoint
) throws
```

## Parameters 

`image`  

CIImage to prepare to render.

`fromRect`  

A CGRect defining the region to render.

`destination`  

The CIRenderDestination to which you are preparing to render.

`atPoint`  

The CGPoint at which you are preparing to render.

`error`  

Pointer to an error should preparation to render fail.

## Return Value

Returns `true` if preparation succeeded.

## Discussion

By making this call, the Core Image framework ensures that any needed kernels are compiled, and any intermediate buffers are allocated and marked volatile up front.

## See Also

### Customizing Render Destination

func startTask(toClear: CIRenderDestination) -> CIRenderTask

Fills the entire destination with black or clear depending on its alphaMode.

func startTask(toRender: CIImage, from: CGRect, to: CIRenderDestination, at: CGPoint) -> CIRenderTask

Renders a portion of an image to a point in the destination.

func startTask(toRender: CIImage, to: CIRenderDestination) -> CIRenderTask

Renders an image to a destination so that point (0, 0) of the image maps to point (0, 0) of the destination.

