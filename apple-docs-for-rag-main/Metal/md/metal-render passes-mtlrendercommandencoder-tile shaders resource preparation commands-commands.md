

- Metal
- Render Passes
- MTLRenderCommandEncoder
-  Tile Shaders Resource Preparation Commands 

API Collection

# Tile Shaders Resource Preparation Commands

Assign resources to tile shaders, including buffers, textures, acceleration structures, sampler states, and function tables.

## Overview

All tile shaders share an argument table for each resource type, such as buffers, textures, and sampler states. These argument tables are separate from other shader types, each of which have their own argument tables, one for each resource type.

## Topics

### Assigning Buffers

func setTileBuffer((any MTLBuffer)?, offset: Int, index: Int)

Assigns a buffer to an entry in the tile shader argument table.

**Required**

func setTileBuffers([(any MTLBuffer)?], offsets: [Int], range: Range&lt;Int>)

Assigns multiple buffers to a range of entries in the tile shader argument table.

func setTileBytes(UnsafeRawPointer, length: Int, index: Int)

Creates a buffer from bytes and assigns it to an entry in the tile shader argument table.

**Required**

func setTileBufferOffset(Int, index: Int)

Updates an entry in the tile shader argument table with a new location within the entry’s current buffer.

**Required**

### Assigning Textures

func setTileTexture((any MTLTexture)?, index: Int)

Assigns a texture to an entry in the tile shader argument table.

**Required**

func setTileTextures([(any MTLTexture)?], range: Range&lt;Int>)

Assigns multiple textures to a range of entries in the tile shader argument table.

### Assigning Sampler States

func setTileSamplerState((any MTLSamplerState)?, index: Int)

Assigns a sampler state to an entry in the tile shader argument table.

**Required**

func setTileSamplerState((any MTLSamplerState)?, lodMinClamp: Float, lodMaxClamp: Float, index: Int)

Assigns a sampler state and clamp values to an entry in the tile shader argument table.

**Required**

func setTileSamplerStates([(any MTLSamplerState)?], range: Range&lt;Int>)

Assigns multiple sampler states to a range of entries in the tile shader argument table.

func setTileSamplerStates([(any MTLSamplerState)?], lodMinClamps: [Float], lodMaxClamps: [Float], range: Range&lt;Int>)

Assigns multiple sampler states and clamp values to a range of entries in the tile shader argument table.

### Assigning Acceleration Structures

func setTileAccelerationStructure((any MTLAccelerationStructure)?, bufferIndex: Int)

Assigns an acceleration structure to an entry in the tile shader argument table.

**Required**

### Assigning Visible Function Tables

func setTileVisibleFunctionTable((any MTLVisibleFunctionTable)?, bufferIndex: Int)

Assigns a visible function table to an entry in the tile shader argument table.

**Required**

func setTileVisibleFunctionTables([(any MTLVisibleFunctionTable)?], bufferRange: Range&lt;Int>)

Assigns multiple visible function tables to a range of entries in the tile shader argument table.

### Assigning Intersection Function Tables

func setTileIntersectionFunctionTable((any MTLIntersectionFunctionTable)?, bufferIndex: Int)

Assigns an intersection function table to an entry in the tile shader argument table.

**Required**

func setTileIntersectionFunctionTables([(any MTLIntersectionFunctionTable)?], bufferRange: Range&lt;Int>)

Assigns multiple intersection function tables to a range of entries in the tile shader argument table.

## See Also

### Encoding Resource Preparation Commands

Mesh and Object Shader Resource Preparation Commands

Assign resources to mesh and object shaders, including buffers, textures, acceleration structures, sampler states, and function tables.

Vertex Shader Resource Preparation Commands

Assign resources to vertex shaders, including buffers, textures, acceleration structures, sampler states, and function tables.

Fragment Shader Resource Preparation Commands

Assign resources to fragment shaders, including buffers, textures, acceleration structures, sampler states, and function tables.

Argument Buffer Resource Preparation Commands

Load individual resources and multiple resources within a heap into GPU memory so that they’re available to shaders through argument buffers.

