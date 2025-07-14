

- Metal
- MTLRenderCommandEncoder
-  setDepthBias(\_:slopeScale:clamp:) 

Instance Method

# setDepthBias(\_:slopeScale:clamp:)

Configures the adjustments a render pass applies to depth values from fragment functions by a scaling factor and bias.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func setDepthBias(
    _ depthBias: Float,
    slopeScale: Float,
    clamp: Float
)
```

**Required**

## Parameters 

`depthBias`  

A constant bias the render pipeline applies to all fragments.

`slopeScale`  

A bias coefficient that scales with the depth of the primitive relative to the camera.

`clamp`  

A value that limits the bias value the render pipeline can apply to a fragment. Pass a positive or negative value to limit the largest magnitude of a positive or negative bias, respectively.

You can disable the bias clamping functionality by passing `0.0`.

## Discussion

Call this method to have the render pipeline apply a bias to the rasterized depth after the clipping stage. The bias affects both depth testing and the values the render pipeline writes to the depth render target. If you don’t explicitly call this method, the pipeline doesn’t apply a scale or a bias to a depth value.

Note

A depth bias only influences triangle primitives, but doesn’t apply to points or lines.

You can use a slope-scaled bias to fine-tune shadow maps and avoid artifacts. Depth artifacts typically come from polygons that exist in the same plane or when a polygon shadows itself, also known as *shadow acne*. The pipeline calculates the bias value differently depending on the data type of the depth pixel format (see MTLPixelFormat).

For unsigned normal or (`Unorm`) pixel formats, the pipeline calculates the bias with a formula that consists of the following definitions:

- The `r` constant is the smallest positive value possible for a depth render target.

- The `maxSlope` variable is the largest possible slope of the depth value at a pixel.

```
bias = (depthBias * r) + (slopeScale * maxSlope)
```

For floating-point (`Float`) pixel formats, the pipeline calculates the bias with a formula that consists of the following definitions:

- The `z` variable is the largest absolute-value vertex depth of the vertices that belong to the primitive.

- The `r` constant is the number of mantissa bits of the floating-point pixel format (not counting the `hidden` bit).

- The `maxSlope` variable is the largest possible slope of the depth value at a pixel.

```
// Get the depth of the vertex within a primitive that has the largest (absolute value) depth.
z = largestAbsoluteDepth(primitive)

// The exponent for 2 is equal to e^(z - r).
exponent = exp(z - r)

// Calculate the bias.
bias = (depthBias * pow(2, exponent)) + (slopeScale * maxSlope)
```

The render pipeline clamps the final bias value if `clamp` isn’t zero.

```
if (clamp > 0.0) {
    bias = min(clamp, bias)
} else if (clamp 

If `clamp` is greater than zero, the pipeline sets the final bias to `clamp` when the formula’s value is greater than `clamp`. If `clamp` is less than zero, the pipeline set the final bias value to `clamp` when the formula’s value is less than `clamp`.

The pipeline adds the final bias value to the depth value, but only if `depthBias` or `slopeScale` is nonzero.

```
if (depthBias != 0.0 || slopeScale != 0.0) {
    depth += bias
}
```

## See Also

### Configuring Depth and Stencil Behavior

func setDepthStencilState((any MTLDepthStencilState)?)

Configures the combined depth and stencil state.

**Required**

func setDepthClipMode(MTLDepthClipMode)

Configures how the render pipeline handles fragments outside the near and far planes of the view frustum.

**Required**

func setStencilReferenceValue(UInt32)

Configures the same comparison value for front- and back-facing primitives.

**Required**

func setStencilReferenceValues(front: UInt32, back: UInt32)

Configures different comparison values for front- and back-facing primitives.

**Required**

