

- Core Services
- Apple Events
-  AEInitializeDesc(\_:) 

Function

# AEInitializeDesc(\_:)

Initializes a new descriptor.

macOS 10.0+

``` source
func AEInitializeDesc(_ desc: UnsafeMutablePointer!)
```

## Parameters 

`desc`  

A pointer to a new descriptor. See AEDesc.

## Discussion

The function sets the type of the descriptor to `typeNull` and sets the data handle to `NULL`. If you need to initialize a descriptor that already has some data in it, use AEDisposeDesc(_:) to deallocate the memory and initialize the descriptor.

### Version-Notes

Thread safe starting in OS X v10.2.

## See Also

### Miscellaneous

func AECheckIsRecord(UnsafePointer&lt;AEDesc>!) -> Bool

Determines whether a descriptor is truly an `AERecord`.

