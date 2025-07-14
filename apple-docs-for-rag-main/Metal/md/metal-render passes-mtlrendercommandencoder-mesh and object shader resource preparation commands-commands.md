

- Metal
- Render Passes
- MTLRenderCommandEncoder
-  Mesh and Object Shader Resource Preparation Commands 

API Collection

# Mesh and Object Shader Resource Preparation Commands

Assign resources to mesh and object shaders, including buffers, textures, acceleration structures, sampler states, and function tables.

## Overview

All mesh shaders share an argument table for each resource type, such as buffers, textures, and sampler states. These argument tables are separate from other shader types, including object shaders, each of which have their own argument tables, one for each resource type.

## Topics

### Assigning Buffers for Object Shaders

func setObjectBuffer((any MTLBuffer)?, offset: Int, index: Int)

Assigns a buffer to an entry in the object shader argument table.

**Required**

func setObjectBuffers([(any MTLBuffer)?], offsets: [Int], range: Range&lt;Int>)

Assigns multiple buffers to a range of entries in the object shader argument table.

func setObjectBytes(UnsafeRawPointer, length: Int, index: Int)

Creates a buffer from bytes and assigns it to an entry in the object shader argument table.

**Required**

func setObjectBufferOffset(Int, index: Int)

Updates an entry in the object shader argument table with a new location within the entry’s current buffer.

**Required**

### Assigning Textures for Object Shaders

func setObjectTexture((any MTLTexture)?, index: Int)

Assigns a texture to an entry in the object shader argument table.

**Required**

func setObjectTextures([(any MTLTexture)?], range: Range&lt;Int>)

Assigns multiple textures to a range of entries in the object shader argument table.

### Assigning Sampler States for Object Shaders

func setObjectSamplerState((any MTLSamplerState)?, index: Int)

Assigns a sampler state to an entry in the object shader argument table.

**Required**

func setObjectSamplerState((any MTLSamplerState)?, lodMinClamp: Float, lodMaxClamp: Float, index: Int)

Assigns a sampler state and clamp values to an entry in the object shader argument table.

**Required**

func setObjectSamplerStates([(any MTLSamplerState)?], range: Range&lt;Int>)

Assigns multiple sampler states to a range of entries in the object shader argument table.

func setObjectSamplerStates([(any MTLSamplerState)?], lodMinClamps: [Float], lodMaxClamps: [Float], range: Range&lt;Int>)

Assigns multiple sampler states and clamp values to a range of entries in the object shader argument table.

### Assigning Buffers for Mesh Shaders

func setMeshBuffer((any MTLBuffer)?, offset: Int, index: Int)

Assigns a buffer to an entry in the mesh shader argument table.

**Required**

func setMeshBuffers([(any MTLBuffer)?], offsets: [Int], range: Range&lt;Int>)

Assigns multiple buffers to a range of entries in the mesh shader argument table.

func setMeshBytes(UnsafeRawPointer, length: Int, index: Int)

Creates a buffer from bytes and assigns it to an entry in the mesh shader argument table.

**Required**

func setMeshBufferOffset(Int, index: Int)

Updates an entry in the mesh shader argument table with a new location within the entry’s current buffer.

**Required**

### Assigning Textures for Mesh Shaders

func setMeshTexture((any MTLTexture)?, index: Int)

Assigns a texture to an entry in the mesh shader argument table.

**Required**

func setMeshTextures([(any MTLTexture)?], range: Range&lt;Int>)

Assigns multiple textures to a range of entries in the mesh shader argument table.

### Assigning Sampler States for Mesh Shaders

func setMeshSamplerState((any MTLSamplerState)?, index: Int)

Assigns a sampler state to an entry in the mesh shader argument table.

**Required**

func setMeshSamplerState((any MTLSamplerState)?, lodMinClamp: Float, lodMaxClamp: Float, index: Int)

Assigns a sampler state and clamp values to an entry in the mesh shader argument table.

**Required**

func setMeshSamplerStates([(any MTLSamplerState)?], range: Range&lt;Int>)

Assigns multiple sampler states to a range of entries in the mesh shader argument table.

func setMeshSamplerStates([(any MTLSamplerState)?], lodMinClamps: [Float], lodMaxClamps: [Float], range: Range&lt;Int>)

Assigns multiple sampler states and clamp values to a range of entries in the mesh shader argument table.

## See Also

### Encoding Resource Preparation Commands

Vertex Shader Resource Preparation Commands

Assign resources to vertex shaders, including buffers, textures, acceleration structures, sampler states, and function tables.

Fragment Shader Resource Preparation Commands

Assign resources to fragment shaders, including buffers, textures, acceleration structures, sampler states, and function tables.

Tile Shaders Resource Preparation Commands

Assign resources to tile shaders, including buffers, textures, acceleration structures, sampler states, and function tables.

Argument Buffer Resource Preparation Commands

Load individual resources and multiple resources within a heap into GPU memory so that they’re available to shaders through argument buffers.

