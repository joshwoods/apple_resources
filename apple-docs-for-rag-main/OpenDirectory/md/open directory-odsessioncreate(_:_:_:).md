

- Open Directory
-  ODSessionCreate(\_:\_:\_:) 

Function

# ODSessionCreate(\_:\_:\_:)

Creates a session to be passed to node functions.

Mac CatalystmacOS 10.6+

``` source
func ODSessionCreate(
    _ allocator: CFAllocator!,
    _ options: CFDictionary!,
    _ error: UnsafeMutablePointer?>!
) -> Unmanaged!
```

## Parameters 

`allocator`  

The memory allocator to use. If `NULL`, the default allocator is used.

`options`  

A dictionary of options to associate with the session.

`error`  

An error reference for error details. Can be `NULL`.

## Return Value

The created session.

## See Also

### Related Documentation

Session Keys

Keys used when specifying session information.

### Working with Sessions

func ODSessionCopyNodeNames(CFAllocator!, ODSessionRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFArray>!

Returns the names of nodes registered in a given session.

func ODSessionGetTypeID() -> CFTypeID

Returns the type ID for a session.

