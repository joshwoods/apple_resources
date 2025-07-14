

- Metal
- MTLStorageMode
-  MTLStorageMode.private 

Case

# MTLStorageMode.private

The resource is only available to the GPU.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
case `private`
```

## Mentioned in 

Choosing a Resource Storage Mode for Intel and AMD GPUs

Choosing a Resource Storage Mode for Apple GPUs

Adjusting for GPU Memory Bandwidth Tradeoffs

Copying Data to a Private Resource

Creating a Counter Sample Buffer to Store a GPU’s Counter Data During a Pass

## Discussion

Metal may apply additional optimizations to private resources that aren’t allowed on shared or managed resources.

For more guidance on how to choose storage modes, see Setting Resource Storage Modes.

## See Also

### Storage Mode Options

case shared

The CPU and GPU share access to the resource, allocated in system memory.

case managed

The CPU and GPU may maintain separate copies of the resource, and any changes must be explicitly synchronized.

case memoryless

The resource’s contents are only available to the GPU, and only exist temporarily during a render pass.

