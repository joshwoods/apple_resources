

- Open Directory
-  ODSessionGetTypeID() 

Function

# ODSessionGetTypeID()

Returns the type ID for a session.

Mac CatalystmacOS 10.6+

``` source
func ODSessionGetTypeID() -> CFTypeID
```

## Return Value

The type ID for a session.

## See Also

### Working with Sessions

func ODSessionCopyNodeNames(CFAllocator!, ODSessionRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFArray>!

Returns the names of nodes registered in a given session.

func ODSessionCreate(CFAllocator!, CFDictionary!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;ODSessionRef>!

Creates a session to be passed to node functions.

