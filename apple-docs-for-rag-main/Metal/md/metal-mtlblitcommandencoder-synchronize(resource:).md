

- Metal
- MTLBlitCommandEncoder
-  synchronize(resource:) 

Instance Method

# synchronize(resource:)

Encodes a command that synchronizes the CPU’s copy of a managed resource, such as a buffer or texture, so that it matches the GPU’s copy.

Mac Catalyst 13.0+macOS 10.11+

``` source
func synchronize(resource: any MTLResource)
```

**Required**

## Parameters 

`resource`  

An MTLResource instance — such as an MTLBuffer or MTLTexture — with a storageMode property that’s equal to MTLStorageMode.managed.

## Mentioned in 

Synchronizing a Managed Resource in macOS

## Discussion

This method ensures the CPU can correctly read all the changes a GPU makes to a resource that uses the managed storage mode. For the resources you create with MTLStorageMode.managed, the CPU and GPU each have a copy of that resource. As the GPU modifies its copy, the CPU’s copy remains unchanged until you synchronize with a command, such as this one.

The CPU can access the updated content from its copy of the resources after the synchronization command completes.

Note

You can encode a command that selectively synchronizes parts of an MTLTexture by calling the synchronize(texture:slice:level:) method.

## See Also

### Working with Managed Resources

func synchronize(texture: any MTLTexture, slice: Int, level: Int)

Encodes a command that synchronizes a part of the CPU’s copy of a texture so that it matches the GPU’s copy.

**Required**

