

- Metal
- MTLRenderCommandEncoder
-  setFrontFacing(\_:) 

Instance Method

# setFrontFacing(\_:)

Configures which face of a primitive, such as a triangle, is the front.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func setFrontFacing(_ frontFacingWinding: MTLWinding)
```

**Required**

## Parameters 

`frontFacingWinding`  

An MTLWinding value that configures how the render pipeline defines which side of a primitive is its front.

## Discussion

The render pass’s default front-facing mode is MTLWinding.clockwise.

The winding direction of a primitive determines whether the render pass culls it (see setCullMode(_:)).

## See Also

### Configuring Rendering Behavior

func setTriangleFillMode(MTLTriangleFillMode)

Configures how subsequent draw commands rasterize triangle and triangle strip primitives.

**Required**

func setCullMode(MTLCullMode)

Configures how the render pipeline determines which primitives to remove.

**Required**

