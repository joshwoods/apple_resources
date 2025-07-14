

- Metal
- MTLStorageMode
-  MTLStorageMode.memoryless 

Case

# MTLStorageMode.memoryless

The resource’s contents are only available to the GPU, and only exist temporarily during a render pass.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+macOS 11.0+tvOS 10.0+visionOS 1.0+

``` source
case memoryless
```

## Mentioned in 

Choosing a Resource Storage Mode for Apple GPUs

Setting Resource Storage Modes

Reducing the Memory Footprint of Metal Apps

## Discussion

The memoryless storage mode uses tile memory, and is only available on Apple family GPUs. Memoryless resources are temporary targets used in a pass and you can’t access their contents with MTLLoadAction.load or MTLStoreAction.store.

Use memoryless resources for temporary elements used only within a single pass. For example, most render passes don’t store depth attachments and multisample attachments to memory. You can significantly reduce your memory usage by creating these attachments as memoryless resources.

On Metal devices that support tile rendering, you can use imageblocks to manage transient rendering data more flexibly. For more information about imageblock memory and using it with your shader functions, see the Metal Shading Language Specification (PDF) sections 2.11, 4.5, and 5.6.

For more guidance on how to choose storage modes, see Setting Resource Storage Modes.

## See Also

### Storage Mode Options

case shared

The CPU and GPU share access to the resource, allocated in system memory.

case managed

The CPU and GPU may maintain separate copies of the resource, and any changes must be explicitly synchronized.

case `private`

The resource is only available to the GPU.

