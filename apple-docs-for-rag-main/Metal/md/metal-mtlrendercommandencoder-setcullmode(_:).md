

- Metal
- MTLRenderCommandEncoder
-  setCullMode(\_:) 

Instance Method

# setCullMode(\_:)

Configures how the render pipeline determines which primitives to remove.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func setCullMode(_ cullMode: MTLCullMode)
```

**Required**

## Parameters 

`cullMode`  

An MTLCullMode value that configures how the render pipeline determines which primitives to remove from the pipeline.

## Discussion

This method configures which primitives the render pipeline removes, if any, based on the direction of each primitive’s face relative to the scene’s camera. For example, you can correctly cull hidden surfaces on some geometric models, such as a sphere made of filled triangles, if it uses orientable surfaces. A surface is *orientable* if its primitives consistently use the same ordering for its vertices. Metal defines vertex ordering with the MTLWinding type, which includes MTLWinding.clockwise and MTLWinding.counterClockwise. You can tell the render pipeline which direction your primitives face by calling the setFrontFacing(_:) method, which affects the primitives the culling mode removes.

The render pass’s default culling mode is MTLCullMode.none.

## See Also

### Configuring Rendering Behavior

func setTriangleFillMode(MTLTriangleFillMode)

Configures how subsequent draw commands rasterize triangle and triangle strip primitives.

**Required**

func setFrontFacing(MTLWinding)

Configures which face of a primitive, such as a triangle, is the front.

**Required**

