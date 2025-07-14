

- Open Directory
-  ODSessionCopyNodeNames(\_:\_:\_:) 

Function

# ODSessionCopyNodeNames(\_:\_:\_:)

Returns the names of nodes registered in a given session.

Mac CatalystmacOS 10.6+

``` source
func ODSessionCopyNodeNames(
    _ allocator: CFAllocator!,
    _ session: ODSessionRef!,
    _ error: UnsafeMutablePointer?>!
) -> Unmanaged!
```

## Parameters 

`allocator`  

The memory allocator to use. If `NULL`, the default allocator is used.

`session`  

The session.

`error`  

An error reference for error details. Can be `NULL`.

## Return Value

An array of valid node names in the given session.

## See Also

### Working with Sessions

func ODSessionCreate(CFAllocator!, CFDictionary!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;ODSessionRef>!

Creates a session to be passed to node functions.

func ODSessionGetTypeID() -> CFTypeID

Returns the type ID for a session.

