

- Metal
- MTLResourceOptions
-  storageModePrivate 

Type Property

# storageModePrivate

The resource is only available to the GPU.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
static var storageModePrivate: MTLResourceOptions { get }
```

## Discussion

Metal may apply additional optimizations to private resources that aren’t allowed on shared or managed resources.

For more guidance on how to choose storage modes, see Setting Resource Storage Modes.

## See Also

### Specifying Storage Modes

static var storageModeShared: MTLResourceOptions

The CPU and GPU share access to the resource, allocated in system memory.

static var storageModeManaged: MTLResourceOptions

The CPU and GPU may maintain separate copies of the resource, and any changes must be explicitly synchronized.

static var storageModeMemoryless: MTLResourceOptions

The resource’s contents are only available to the GPU, and only exist temporarily during a render pass.

