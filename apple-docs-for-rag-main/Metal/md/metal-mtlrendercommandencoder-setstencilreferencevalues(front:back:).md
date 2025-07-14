

- Metal
- MTLRenderCommandEncoder
-  setStencilReferenceValues(front:back:) 

Instance Method

# setStencilReferenceValues(front:back:)

Configures different comparison values for front- and back-facing primitives.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func setStencilReferenceValues(
    front frontReferenceValue: UInt32,
    back backReferenceValue: UInt32
)
```

**Required**

## Parameters 

`frontReferenceValue`  

A stencil test comparison value the render pipeline applies to only front-facing primitives.

`backReferenceValue`  

A stencil test comparison value the render pipeline applies to only back-facing primitives.

## Discussion

The command sets separate reference values for front- and back-facing primitives (see stencilCompareFunction, frontFaceStencil, and backFaceStencil). These reference values apply to the stencil state you set with the setDepthStencilState(_:) method.

The render pass’s default reference value for the front and back stencil compare function is `0`.

## See Also

### Configuring Depth and Stencil Behavior

func setDepthStencilState((any MTLDepthStencilState)?)

Configures the combined depth and stencil state.

**Required**

func setDepthBias(Float, slopeScale: Float, clamp: Float)

Configures the adjustments a render pass applies to depth values from fragment functions by a scaling factor and bias.

**Required**

func setDepthClipMode(MTLDepthClipMode)

Configures how the render pipeline handles fragments outside the near and far planes of the view frustum.

**Required**

func setStencilReferenceValue(UInt32)

Configures the same comparison value for front- and back-facing primitives.

**Required**

