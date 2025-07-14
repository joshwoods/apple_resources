

- Metal
- MTLRenderCommandEncoder
-  setTriangleFillMode(\_:) 

Instance Method

# setTriangleFillMode(\_:)

Configures how subsequent draw commands rasterize triangle and triangle strip primitives.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func setTriangleFillMode(_ fillMode: MTLTriangleFillMode)
```

**Required**

## Parameters 

`fillMode`  

A triangle filling mode the render pass applies to draw commands that rasterize triangles or triangle strips.

## Discussion

The render pass’s default mode is MTLTriangleFillMode.fill.

## See Also

### Configuring Rendering Behavior

func setFrontFacing(MTLWinding)

Configures which face of a primitive, such as a triangle, is the front.

**Required**

func setCullMode(MTLCullMode)

Configures how the render pipeline determines which primitives to remove.

**Required**

