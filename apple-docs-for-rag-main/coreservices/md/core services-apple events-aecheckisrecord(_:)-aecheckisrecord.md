

- Core Services
- Apple Events
-  AECheckIsRecord(\_:) 

Function

# AECheckIsRecord(\_:)

Determines whether a descriptor is truly an `AERecord`.

macOS 10.0+

``` source
func AECheckIsRecord(_ theDesc: UnsafePointer!) -> Bool
```

## Parameters 

`theDesc`  

A pointer to the descriptor to check.

## Return Value

Returns `true` if the descriptor is an `AERecord` or an `AppleEvent`, `false` otherwise.

## Discussion

Thread safe starting in OS X v10.2.

## See Also

### Miscellaneous

func AEInitializeDesc(UnsafeMutablePointer&lt;AEDesc>!)

Initializes a new descriptor.

