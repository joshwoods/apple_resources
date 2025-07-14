

- Metal
- Render Passes
- MTLRenderCommandEncoder
-  Fragment Shader Resource Preparation Commands 

API Collection

# Fragment Shader Resource Preparation Commands

Assign resources to fragment shaders, including buffers, textures, acceleration structures, sampler states, and function tables.

## Overview

All fragment shaders share an argument table for each resource type, such as buffers, textures, and sampler states. These argument tables are separate from other shader types, each of which have their own argument tables, one for each resource type.

## Topics

### Assigning Buffers

func setFragmentBuffer((any MTLBuffer)?, offset: Int, index: Int)

Assigns a buffer to an entry in the fragment shader argument table.

**Required**

func setFragmentBuffers([(any MTLBuffer)?], offsets: [Int], range: Range&lt;Int>)

Assigns multiple buffers to a range of entries in the fragment shader argument table.

func setFragmentBytes(UnsafeRawPointer, length: Int, index: Int)

Creates a buffer from bytes and assigns it to an entry in the fragment shader argument table.

**Required**

func setFragmentBufferOffset(Int, index: Int)

Updates an entry in the fragment shader argument table with a new location within the entry’s current buffer.

**Required**

### Assigning Textures

func setFragmentTexture((any MTLTexture)?, index: Int)

Assigns a texture to an entry in the fragment shader argument table.

**Required**

func setFragmentTextures([(any MTLTexture)?], range: Range&lt;Int>)

Assigns multiple textures to a range of entries in the fragment shader argument table.

### Assigning Sampler States

func setFragmentSamplerState((any MTLSamplerState)?, index: Int)

Assigns a sampler state to an entry in the fragment shader argument table.

**Required**

func setFragmentSamplerState((any MTLSamplerState)?, lodMinClamp: Float, lodMaxClamp: Float, index: Int)

Assigns a sampler state and clamp values to an entry in the fragment shader argument table.

**Required**

func setFragmentSamplerStates([(any MTLSamplerState)?], range: Range&lt;Int>)

Assigns multiple sampler states to a range of entries in the fragment shader argument table.

func setFragmentSamplerStates([(any MTLSamplerState)?], lodMinClamps: [Float], lodMaxClamps: [Float], range: Range&lt;Int>)

Assigns multiple sampler states and clamp values to a range of entries in the fragment shader argument table.

### Assigning Acceleration Structures

func setFragmentAccelerationStructure((any MTLAccelerationStructure)?, bufferIndex: Int)

Assigns an acceleration structure to an entry in the fragment shader argument table.

**Required**

### Assigning Visible Function Tables

func setFragmentVisibleFunctionTable((any MTLVisibleFunctionTable)?, bufferIndex: Int)

Assigns a visible function table to an entry in the fragment shader argument table.

**Required**

func setFragmentVisibleFunctionTables([(any MTLVisibleFunctionTable)?], bufferRange: Range&lt;Int>)

Assigns multiple visible function tables to a range of entries in the fragment shader argument table.

### Assigning Intersection Function Tables

func setFragmentIntersectionFunctionTable((any MTLIntersectionFunctionTable)?, bufferIndex: Int)

Assigns an intersection function table to an entry in the fragment shader argument table.

**Required**

func setFragmentIntersectionFunctionTables([(any MTLIntersectionFunctionTable)?], bufferRange: Range&lt;Int>)

Assigns multiple intersection function tables to a range of entries in the fragment shader argument table.

## See Also

### Encoding Resource Preparation Commands

Mesh and Object Shader Resource Preparation Commands

Assign resources to mesh and object shaders, including buffers, textures, acceleration structures, sampler states, and function tables.

Vertex Shader Resource Preparation Commands

Assign resources to vertex shaders, including buffers, textures, acceleration structures, sampler states, and function tables.

Tile Shaders Resource Preparation Commands

Assign resources to tile shaders, including buffers, textures, acceleration structures, sampler states, and function tables.

Argument Buffer Resource Preparation Commands

Load individual resources and multiple resources within a heap into GPU memory so that they’re available to shaders through argument buffers.

