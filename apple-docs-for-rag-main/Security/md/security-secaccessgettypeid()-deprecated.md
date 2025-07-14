

- Security
-  SecAccessGetTypeID() Deprecated

Function

# SecAccessGetTypeID()

Returns the unique identifier of the opaque type to which an access instance belongs.

macOS 10.2–10.10Deprecated

``` source
func SecAccessGetTypeID() -> CFTypeID
```

Deprecated

SecKeychain is deprecated

## Return Value

A value that identifies the opaque type of a SecAccess instance.

## Discussion

This method returns a value that uniquely identifies the opaque type of a SecAccess instance. You can compare this value to the CFTypeID identifier obtained by calling the CFGetTypeID(_:) method on a specific object. These values might change from release to release or platform to platform.

