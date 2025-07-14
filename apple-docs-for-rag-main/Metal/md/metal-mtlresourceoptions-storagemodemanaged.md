

- Metal
- MTLResourceOptions
-  storageModeManaged 

Type Property

# storageModeManaged

The CPU and GPU may maintain separate copies of the resource, and any changes must be explicitly synchronized.

Mac Catalyst 13.0+macOS 10.11+

``` source
static var storageModeManaged: MTLResourceOptions { get }
```

## Discussion

On Intel-based Mac computers, this is the default storage mode for MTLTexture objects. In iOS and tvOS, the managed storage mode isn’t available. With managed storage, you synchronize changes between the CPU and GPU manually. For instructions and examples of resource synchronization, see Synchronizing a Managed Resource in macOS.

For more guidance on how to choose storage modes, see Setting Resource Storage Modes.

## See Also

### Specifying Storage Modes

static var storageModeShared: MTLResourceOptions

The CPU and GPU share access to the resource, allocated in system memory.

static var storageModePrivate: MTLResourceOptions

The resource is only available to the GPU.

static var storageModeMemoryless: MTLResourceOptions

The resource’s contents are only available to the GPU, and only exist temporarily during a render pass.

