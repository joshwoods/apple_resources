

- Metal
- MTLStorageMode
-  MTLStorageMode.shared 

Case

# MTLStorageMode.shared

The CPU and GPU share access to the resource, allocated in system memory.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
case shared
```

## Mentioned in 

Optimizing Texture Data

Choosing a Resource Storage Mode for Apple GPUs

Setting Resource Storage Modes

Choosing a Resource Storage Mode for Intel and AMD GPUs

Synchronizing a Managed Resource in macOS

## Discussion

This is the default storage mode for MTLBuffer instances on integrated GPUs and both MTLBuffer and MTLTexture instances on Apple silicon GPUs. On non-Apple family GPUs, the shared storage mode isn’t available for MTLTexture instances.

When either the CPU or GPU changes the contents of the resource, you’re responsible for synchronizing access to the texture from the other participant. Ensure that all changes you schedule on either the CPU or GPU for a resource that uses shared memory complete before accessing that resource on the other processor.

For more guidance on how to choose storage modes, see Setting Resource Storage Modes.

## See Also

### Storage Mode Options

case managed

The CPU and GPU may maintain separate copies of the resource, and any changes must be explicitly synchronized.

case `private`

The resource is only available to the GPU.

case memoryless

The resource’s contents are only available to the GPU, and only exist temporarily during a render pass.

