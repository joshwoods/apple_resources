

- Metal
- MTLBlitCommandEncoder
-  synchronize(texture:slice:level:) 

Instance Method

# synchronize(texture:slice:level:)

Encodes a command that synchronizes a part of the CPU’s copy of a texture so that it matches the GPU’s copy.

Mac Catalyst 13.0+macOS 10.11+

``` source
func synchronize(
    texture: any MTLTexture,
    slice: Int,
    level: Int
)
```

**Required**

## Parameters 

`texture`  

An MTLTexture instance with a storageMode property that’s equal to MTLStorageMode.managed.

`slice`  

A slice within `texture`.

`level`  

A mipmap level within `texture`.

## Mentioned in 

Synchronizing a Managed Resource in macOS

## Discussion

This method ensures the CPU can correctly read the changes a GPU makes to a slice of a texture that uses the managed storage mode. For the resources you create with MTLStorageMode.managed, the CPU and GPU each have a copy of that resource. As the GPU modifies its copy, the CPU’s copy remains unchanged until you synchronize with a command, such as this one.

The CPU can access the updated content from its copy of the texture after the synchronization command completes.

Note

The command this method encodes behaves similarly to the command that synchronize(resource:) encodes, except that it flushes only the applicable slice and mipmap level.

## See Also

### Working with Managed Resources

func synchronize(resource: any MTLResource)

Encodes a command that synchronizes the CPU’s copy of a managed resource, such as a buffer or texture, so that it matches the GPU’s copy.

**Required**

