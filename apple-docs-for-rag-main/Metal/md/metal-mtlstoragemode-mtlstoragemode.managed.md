

- Metal
- MTLStorageMode
-  MTLStorageMode.managed 

Case

# MTLStorageMode.managed

The CPU and GPU may maintain separate copies of the resource, and any changes must be explicitly synchronized.

Mac Catalyst 13.0+macOS 10.11+

``` source
case managed
```

## Mentioned in 

Synchronizing a Managed Resource in macOS

Optimizing Texture Data

Setting Resource Storage Modes

Choosing a Resource Storage Mode for Intel and AMD GPUs

Adjusting for GPU Memory Bandwidth Tradeoffs

## Discussion

On Intel-based Mac computers, this is the default storage mode for MTLTexture objects. In iOS and tvOS, the managed storage mode isn’t available. With managed storage, you synchronize changes between the CPU and GPU manually. For instructions and examples of resource synchronization, see Synchronizing a Managed Resource in macOS.

For more guidance on how to choose storage modes, see Setting Resource Storage Modes.

## See Also

### Storage Mode Options

case shared

The CPU and GPU share access to the resource, allocated in system memory.

case `private`

The resource is only available to the GPU.

case memoryless

The resource’s contents are only available to the GPU, and only exist temporarily during a render pass.

