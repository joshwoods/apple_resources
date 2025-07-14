

- RealityKit
-  LowLevelTexture 

Class

# LowLevelTexture

A container for texture data allowing you to create and update textures using your own format.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor
class LowLevelTexture
```

## Mentioned in 

Creating a dynamic height and normal map with low-level texture

## Overview

Use `LowLevelTexture` when you want to bring your own texture data to RealityKit, or update your data frequently. You update the data on the GPU with Metal compute shaders. This is ideal for bringing your own textures to RealityKit as-is, or when you intend to update your data frequently.

Note

For a simpler alternative, consider creating your TextureResource from a CGImage with init(image:withName:options:), texture2DArray(slices:named:options:), cube(slices:named:options:), or texture3D(slices:named:options:).

Express your texture by creating a LowLevelTexture.Descriptor that describes how the data is laid out, along with the size of the texture. This descriptor is similar to MTLTextureDescriptor.

To use `LowLevelTexture`, first configure the descriptor with the desired characteristics of your texture.

```
var textureDescriptor: LowLevelTexture.Descriptor {
    var desc = LowLevelTexture.Descriptor()

    desc.textureType = .type2D
    desc.arrayLength = 1

    desc.width = 2048
    desc.height = 2048
    desc.depth = 1

    desc.mipmapLevelCount = 1
    desc.pixelFormat = .bgra8Unorm
    desc.textureUsage = [.shaderRead, .shaderWrite]
    desc.swizzle = .init(red: .red, green: .green, blue: .blue, alpha: .alpha)

    return desc
}
```

Then, you can initialize the `LowLevelTexture` from its descriptor and provide it to a TextureResource.

```
let texture = try LowLevelTexture(descriptor: textureDescriptor)
let resource = try TextureResource(from: texture)
```

You update the contents of a `LowLevelTexture` on the GPU, using a Metal Command Buffer and Compute Command Encoder. For example, you can write a compute kernel in Metal Shading Language to generate the color of each pixel:

```
kernel void
lowLevelTextureKernel(
    texture2d outTexture [[texture(0)]],
    uint2 gid [[thread_position_in_grid]])
{
    // Compute texture coordinate ranging from 0 to 1 along each axis.
    half2 texCoord {
        half(gid[0]) / (outTexture.get_width() - 1),
        half(gid[1]) / (outTexture.get_height() - 1)
    };

    // Compute the color as a linear gradient from top to bottom.
    half3 color = mix(
        half3 { 0.2, 0.2, 0.8 },
        half3 { 0.7, 0.7, 0.9 },
        texCoord.y);

    // Specify an opacity of 1 if the pixel is within a circle
    // spanning the image bounds.
    half alpha = length(texCoord - 0.5) 

You can use this compute kernel to populate the `LowLevelTexture`:

```
func populate(texture: LowLevelTexture, device: MTLDevice) {
    // Set up the Metal command queue and compute command encoder, 
    // or abort if that fails.
    guard let commandQueue = device.makeCommandQueue(),
          let commandBuffer = commandQueue.makeCommandBuffer(),
          let computeEncoder = commandBuffer.makeComputeCommandEncoder() else {
        return
    }

    // Load a Metal compute kernel written in Metal Shading Language, 
    // or abort if that fails.
    guard let library = device.makeDefaultLibrary(),
          let function = library.makeFunction(name: "lowLevelTextureKernel"),
          let computePipelineState = try? device.makeComputePipelineState(function: function) else {
        return
    }

    // Enqueue the Metal command buffer.
    commandBuffer.enqueue()

    // Set up the Metal compute command encoder with the app's compute kernel.
    computeEncoder.setComputePipelineState(computePipelineState)

    // Retrieve a MTLTexture from LowLevelTexture.
    // This texture will be directly consumed by RealityKit's renderer.
    let outTexture: MTLTexture = texture.replace(using: commandBuffer)
    computeEncoder.setTexture(outTexture, index: 0)

    // Disptach the GPU compute work.
    // Note: threadGroupCount and threadGroupSize determined elsewhere.
    computeEncoder.dispatchThreadgroups(
        threadGroupCount,
        threadsPerThreadgroup: threadGroupSize)

    // End the encoding and commit the command buffer.
    // When the command buffer completes, RealityKit automatically applies the changes.
    computeEncoder.endEncoding()
    commandBuffer.commit()
}
```

To finish, add your TextureResource to a Material and display it on an Entity.

```
func textureEntity(device: MTLDevice) throws -> Entity {
    // Create the LowLevelTexture and populate it on the GPU.
    let texture = try LowLevelTexture(descriptor: textureDescriptor)
    populate(texture: texture, device: device)

    // Create a TextureResource from the LowLevelTexture.
    let resource = try TextureResource(from: texture)

    // Create a material that uses the texture.
    var material = UnlitMaterial(texture: resource)
    material.opacityThreshold = 0.5

    // Return an entity of a plane which uses the generated texture.
    return ModelEntity(mesh: .generatePlane(width: 1, depth: 1), materials: [material])
}
```

The TextureResource retains a reference to the `LowLevelTexture`, and presents changes made to the `LowLevelTexture` when the renderer updates.

## Topics

### Structures

struct Descriptor

An object that you use to configure new `LowLevelTexture` objects.

### Initializers

init(descriptor: LowLevelTexture.Descriptor) throws

Creates a low-level texture from a descriptor.

### Instance Properties

let descriptor: LowLevelTexture.Descriptor

The descriptor that you use to initialize the `LowLevelTexture`.

### Instance Methods

func read() -> any MTLTexture

Retrieves the current texture for GPU reading.

func replace(using: any MTLCommandBuffer) -> any MTLTexture

Retrieves a Metal texture that your app’s shaders can write to when they run on a GPU.

## Relationships

### Conforms To

- Sendable

## See Also

### Texture drawing

Rendering a windowed game in stereo

Bring an iOS or iPadOS game to visionOS and enhance it.

Creating a dynamic height and normal map with low-level texture

Create a low-level texture and update its pixel data on the GPU to form a dynamic height and normal map.

struct Descriptor

An object that you use to configure new `LowLevelTexture` objects.

class Drawable

A drawable associated with a drawable queue

class DrawableQueue

A drawable queue that may be used to update a texture resource dynamically

struct Descriptor

Describes the texture managed by the drawable queue

