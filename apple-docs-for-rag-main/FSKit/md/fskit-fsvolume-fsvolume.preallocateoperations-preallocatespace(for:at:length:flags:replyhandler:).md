

- FSKit
- FSVolume
- FSVolume.PreallocateOperations
-  preallocateSpace(for:at:length:flags:replyHandler:) 

Instance Method

# preallocateSpace(for:at:length:flags:replyHandler:)

Prealocates disk space for the given item.

macOS 15.4+

``` source
func preallocateSpace(
    for item: FSItem,
    at offset: off_t,
    length: Int,
    flags: FSVolume.PreallocateFlags,
    replyHandler reply: @escaping (Int, (any Error)?) -> Void
)
```

``` source
func preallocateSpace(
    for item: FSItem,
    at offset: off_t,
    length: Int,
    flags: FSVolume.PreallocateFlags
) async throws -> Int
```

**Required**

## Parameters 

`item`  

The item for which to preallocate space.

`offset`  

The offset from which to allocate.

`length`  

The length of the space in bytes.

`flags`  

Flags that affect the preallocation behavior.

`reply`  

A block or closure to indicate success or failure. If preallocation succeeds, pass the amount of bytes allocated and a `nil` error. If preallocation fails, pass the relevant error as the second parameter; FSKit ignores any byte count in this case. For an `async` Swift implementation, there’s no reply handler; simply return the allocated byte count or throw an error.

## See Also

### Preallocating space

struct PreallocateFlags

Behavior flags for preallocation operations.

