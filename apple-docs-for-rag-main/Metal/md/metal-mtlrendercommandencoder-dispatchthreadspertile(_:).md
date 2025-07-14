

- Metal
- MTLRenderCommandEncoder
-  dispatchThreadsPerTile(\_:) 

Instance Method

# dispatchThreadsPerTile(\_:)

Encodes a command that invokes GPU functions from the encoder’s current tile render pipeline state.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.5+visionOS 1.0+

``` source
func dispatchThreadsPerTile(_ threadsPerTile: MTLSize)
```

**Required**

## Parameters 

`threadsPerTile`  

An MTLSize instance that represents the number of threads the render pass uses per tile.

Set the size’s width and height properties to values that are less than or equal to tileWidth and tileHeight, respectively. Some GPU families only support square tile dispatches and require the same value for width and height. See the Metal feature set tables (PDF) to check which GPU families support nonsquare dispatches.

Set the depth property to `1`.

## Discussion

The command invokes the GPU function that’s in the encoder’s current tile render pipeline state. You can configure that state with the following steps:

1.  Configure an MTLTileRenderPipelineDescriptor instance.

2.  Create a tile render pipeline state by calling one of the applicable methods of an MTLDevice instance, including makeRenderPipelineState(tileDescriptor:options:reflection:).

3.  Apply that tile render pipeline state by calling the setRenderPipelineState(_:) method.

The method records the encoder’s current rendering state and resources the command needs as it runs. You can safely change the encoder’s render pipeline state to encode other commands after calling this method. Subsequent changes to the state don’t affect the commands already in the encoder’s MTLCommandBuffer.

## See Also

### Drawing with Tile Shaders

var tileWidth: Int

The width of the tiles, in pixels, for the render command encoder.

**Required**

var tileHeight: Int

The height of the tiles, in pixels, for the render command encoder.

**Required**

