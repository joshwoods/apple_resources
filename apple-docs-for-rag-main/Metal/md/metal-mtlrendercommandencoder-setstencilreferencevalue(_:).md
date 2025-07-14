

- Metal
- MTLRenderCommandEncoder
-  setStencilReferenceValue(\_:) 

Instance Method

# setStencilReferenceValue(\_:)

Configures the same comparison value for front- and back-facing primitives.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func setStencilReferenceValue(_ referenceValue: UInt32)
```

**Required**

## Parameters 

`referenceValue`  

A stencil test comparison value the render pipeline applies to both front- and back-facing primitives.

## Discussion

The command sets the same reference value for front- and back-facing primitives (see stencilCompareFunction, frontFaceStencil, and backFaceStencil). This reference value applies to the stencil state you set with the setDepthStencilState(_:) method.

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

func setStencilReferenceValues(front: UInt32, back: UInt32)

Configures different comparison values for front- and back-facing primitives.

**Required**

