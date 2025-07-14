

- Metal
- MTLRenderCommandEncoder
-  setDepthClipMode(\_:) 

Instance Method

# setDepthClipMode(\_:)

Configures how the render pipeline handles fragments outside the near and far planes of the view frustum.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.11+tvOS 11.0+visionOS 1.0+

``` source
func setDepthClipMode(_ depthClipMode: MTLDepthClipMode)
```

**Required**

## Parameters 

`depthClipMode`  

The mode that determines how to handle fragments outside the near and far planes.

## Discussion

You can use depth clipping to ignore fragments outside the z-axis boundaries of a viewing volume.

The render pass’s default clip mode is MTLDepthClipMode.clip.

## See Also

### Configuring Depth and Stencil Behavior

func setDepthStencilState((any MTLDepthStencilState)?)

Configures the combined depth and stencil state.

**Required**

func setDepthBias(Float, slopeScale: Float, clamp: Float)

Configures the adjustments a render pass applies to depth values from fragment functions by a scaling factor and bias.

**Required**

func setStencilReferenceValue(UInt32)

Configures the same comparison value for front- and back-facing primitives.

**Required**

func setStencilReferenceValues(front: UInt32, back: UInt32)

Configures different comparison values for front- and back-facing primitives.

**Required**

