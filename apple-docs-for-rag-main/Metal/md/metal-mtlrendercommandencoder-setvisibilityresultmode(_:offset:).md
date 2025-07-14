

- Metal
- MTLRenderCommandEncoder
-  setVisibilityResultMode(\_:offset:) 

Instance Method

# setVisibilityResultMode(\_:offset:)

Configures which visibility test the GPU runs and the destination for any results it generates.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func setVisibilityResultMode(
    _ mode: MTLVisibilityResultMode,
    offset: Int
)
```

**Required**

## Parameters 

`mode`  

An MTLVisibilityResultMode that configures which visibility test results the render pass saves to a buffer, or disables visibility testing.

`offset`  

A location, in bytes, relative to the start of the render pass’s visibilityResultBuffer. The GPU stores the result of a visibility test at `offset`, which needs to be a multiple of 8.

## Discussion

To create a render pass that can enable visibility testing, assign an MTLBuffer instance to the visibilityResultBuffer property of an MTLRenderPassDescriptor.

You can monitor one or more drawing commands with a visibility test by calling this method before the drawing commands. The encoder uses the new visibility mode and offset for subsequent drawing commands until you change the configuration by calling the method again. For example, you can change the offset or entirely disable visibility tests for subsequent commands by passing MTLVisibilityResultMode.disabled.

Note

You can set a specific `offset` value only once per render pass. This means you need to encode all drawing commands for an offset at one time.

The default mode for a render pass is MTLVisibilityResultMode.disabled.

