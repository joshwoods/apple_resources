

- Metal
- Buffers
-  Using Argument Buffers with Resource Heaps 

Sample Code

# Using Argument Buffers with Resource Heaps

Reduce CPU overhead by using arrays inside argument buffers and combining them with resource heaps.

Download

iOS 12.0+iPadOS 12.0+macOS 10.13+tvOS 12.0+Xcode 12.3+

## Overview

In the Managing Groups of Resources with Argument Buffers sample, you learned how to specify, encode, set, and access resources in an argument buffer.

In this sample, you’ll learn how to combine argument buffers with arrays of resources and resource heaps. In particular, you’ll learn how to define an argument buffer structure that contains arrays and how to allocate and use resources from a heap. The sample renders a static quad that uses multiple resources encoded into an argument buffer.

### Getting Started

The Xcode project contains schemes for running the sample on macOS, iOS, or tvOS. Metal is not supported in the iOS or tvOS Simulator, so the iOS and tvOS schemes require a physical device to run the sample. The default scheme is macOS, which runs the sample as is on your Mac.

### Arrays of Arguments in the Metal Shading Language

Arrays can be used as parameters to graphics or compute functions. When a function takes an array as a parameter, the index of the first resource in the array is equal to the base index of the array parameter itself. Thus, each subsequent resource in the array is automatically assigned a subsequent index value, counting incrementally from the base index value.

For example, the following fragment function, `exampleFragmentFunction`, has a parameter, `textureParameters`, that’s an array of 10 textures with a base index value of `5`.

```
fragment float4
exampleFragmentFunction(array, 10> textureParameters [[ texture(5) ]])
```

Because `textureParameters` has a `[[ texture(5) ]]` attribute qualifier, the corresponding Metal framework method to set this parameter is `setFragmentTexture:atIndex:`, where the values for `index` begin at `5`. Thus, the texture at array index `0` is set at index number `5`, the texture at array index `1` is set at index number `6`, and so on. The last texture in the array, at array index `9`, is set at index number `14`.

### Define Argument Buffers with Arrays

Arrays can also be used as elements of an argument buffer structure. In this case, the `[[ id(n) ]]` attribute qualifier of an argument buffer behaves the same way as the `[[ texture(n) ]]` attribute qualifier of a function parameter, where `n` is the base index value of the array. However, you don’t call the `setFragmentTexture:atIndex:` method, of a `MTLRenderCommandEncoder` object, to set a texture from the array. Instead, you call the `setTexture:atIndex:` method, of a `MTLArgumentEncoder` object, to encode a texture from the array into the argument buffer, where `index` corresponds to the base index value, `n`, plus the index of the texture within the array.

The argument buffer in this sample is declared as a `FragmentShaderArguments` structure, and this is its definition:

```
struct FragmentShaderArguments {
    array, AAPLNumTextureArguments> exampleTextures  [[ id(AAPLArgumentBufferIDExampleTextures)  ]];
    array   exampleBuffers   [[ id(AAPLArgumentBufferIDExampleBuffers)   ]];
    array          exampleConstants [[ id(AAPLArgumentBufferIDExampleConstants) ]];
};
```

Each element of this structure uses the `array` template, which defines the element as an array of a certain type, `T`, and number of elements, `N`. This argument buffer contains the following resources:

- `exampleTextures`, an array of 32 2D textures with a base index value of `0`.

- `exampleBuffers`, an array of 32 `float` buffers with a base index value of `100`.

- `exampleConstants`, an array of 32 `uint32_t` constants with a base index value of `200`.

### Encode Array Elements into an Argument Buffer

This sample encodes array elements into an argument buffer by matching the `index` parameter of each `setTexture:atIndex:`, `setBuffer:offset:atIndex:`, and `constantDataAtIndex:` method call to the element’s corresponding index value, defined by the `[[ id(n) ]]` attribute qualifier in the argument buffer.

```
for(uint32_t i = 0; i 

```
for(uint32_t i = 0; i 

### Access Array Elements in an Argument Buffer

Within a function, accessing elements of an array encoded in an argument buffer is the same as accessing elements of a standard array. In this sample, the `exampleTextures`, `exampleBuffers`, and `exampleConstants` arrays are accessed via the `fragmentShaderArgs` parameter of the `fragmentShader` function. Each array element is accessed with the `[n]` subscript syntax, where `n` is the index of the element within the array.

```
for(uint32_t textureToSample = 0; textureToSample 

The `fragmentShader` function contains an `if-else` condition that evaluates the `x` component of `texCoord` to determine which side of the quad the fragment is on. If the fragment is on the left side of the quad, the function samples each texture in the `exampleTextures` array and adds the sampled values to determine the final output color.

If the fragment is on right side of the quad, the function reads a value from the `exampleBuffers` array. The function uses the `x` component of `texCoord` to determine which buffer to read from and then uses the `y` component of `texCoord` to determine where in the buffer to read from. The value in the buffer determines the final output color.

```
// Use texCoord.x to select the buffer to read from
uint32_t bufferToRead = (in.texCoord.x-0.5)*2.0 * (AAPLNumBufferArguments-1);

// Retrieve the number of elements for the selected buffer from
// the array of constants in the argument buffer
uint32_t numElements = fragmentShaderArgs.exampleConstants[bufferToRead];

// Determine the index used to read from the buffer
uint32_t indexToRead = in.texCoord.y * numElements;

// Retrieve the buffer to read from by accessing the array of
// buffers in the argument buffer
device float* buffer = fragmentShaderArgs.exampleBuffers[bufferToRead];

// Read from the buffer and assign the value to the output color
color = buffer[indexToRead];
```

### Combine Argument Buffers with Resource Heaps

The fragment function accesses 32 textures and 32 buffers via the argument buffer, totaling 64 different resources overall. If memory for each of these resources was allocated individually, despite residing in arrays, Metal would need to validate the memory of 64 individual resources before making these resources accessible to the GPU.

Instead, this sample allocates resources from a `MTLHeap` object. A heap is a single memory region from which multiple resources can be allocated. Therefore, the sample can make the heap’s entire memory, including the memory of all the resources within the heap, accessible to the GPU by calling the `useHeap:` method once.

The sample implements a `loadResources` method that loads the resource data into temporary `MTLTexture` and `MTLBuffer` objects. Then, the sample implements a `createHeap` method that calculates the total size required to store the resource data in the heap and creates the heap itself.

```
- (void) createHeap
{
    MTLHeapDescriptor *heapDescriptor = [MTLHeapDescriptor new];
    heapDescriptor.storageMode = MTLStorageModePrivate;
    heapDescriptor.size =  0;

    // Build a descriptor for each texture and calculate the size required to store all textures in the heap
    for(uint32_t i = 0; i 

The sample implements a `moveResourcesToHeap` method that creates permanent `MTLTexture` and `MTLBuffer` objects allocated from the heap. Then, the method uses a `MTLBlitCommandEncoder` to copy the resource data from the temporary objects to the permanent objects.

```
- (void)moveResourcesToHeap
{
    // Create a command buffer and blit encoder to copy data from the existing resources to
    // the new resources created from the heap
    id  commandBuffer = [_commandQueue commandBuffer];
    commandBuffer.label = @"Heap Copy Command Buffer";

    id  blitEncoder = commandBuffer.blitCommandEncoder;
    blitEncoder.label = @"Heap Transfer Blit Encoder";

    // Create new textures from the heap and copy the contents of the existing textures to
    // the new textures
    for(uint32_t i = 0; i  heapTexture = [_heap newTextureWithDescriptor:descriptor];

        heapTexture.label = _texture[i].label;

        [blitEncoder pushDebugGroup:[NSString stringWithFormat:@"%@ Blits", heapTexture.label]];

        // Blit every slice of every level from the existing texture to the new texture
        MTLRegion region = MTLRegionMake2D(0, 0, _texture[i].width, _texture[i].height);
        for(NSUInteger level = 0; level  heapBuffer = [_heap newBufferWithLength:_dataBuffer[i].length
                                                      options:MTLResourceStorageModePrivate];

        heapBuffer.label = _dataBuffer[i].label;

        // Blit contents of the original buffer to the new buffer
        [blitEncoder copyFromBuffer:_dataBuffer[i]
                       sourceOffset:0
                           toBuffer:heapBuffer
                  destinationOffset:0
                               size:heapBuffer.length];

        // Replace the existing buffer with the new buffer
        _dataBuffer[i] = heapBuffer;
    }

    [blitEncoder endEncoding];
    [commandBuffer commit];
}
```

Before using these resources, instead of calling the `useResource:usage:` method once for each resource, the sample calls the `useHeap:` method once for the entire heap.

```
#if ENABLE_RESOURCE_HEAP
        // Make a single `useHeap:` call for the entire heap, instead of one
        // `useResource:usage:` call per texture and per buffer
        [renderEncoder useHeap:_heap];
#else
        for(uint32_t i = 0; i 

### Next Steps

In this sample, you learned how to combine argument buffers with arrays of resources and resource heaps. In the Encoding Argument Buffers on the GPU sample, you’ll learn how to encode resources into argument buffers with a graphics or compute function.

## See Also

### Argument Buffers

Improving CPU Performance by Using Argument Buffers

Optimize your app’s performance by grouping your resources into argument buffers.

Managing groups of resources with argument buffers

Create argument buffers to organize related resources.

Tracking the Resource Residency of Argument Buffers

Optimize resource performance within an argument buffer.

Indexing Argument Buffers

Assign resource indices within an argument buffer.

Rendering Terrain Dynamically with Argument Buffers

Use argument buffers to render terrain in real time with a GPU-driven pipeline.

Encoding Argument Buffers on the GPU

Use a compute pass to encode an argument buffer and access its arguments in a subsequent render pass.

class MTLArgumentDescriptor

A representation of an argument within an argument buffer.

protocol MTLArgumentEncoder

An object used to encode data into an argument buffer.

let MTLAttributeStrideStatic: Int

