

- Security
-  SecACLGetTypeID() Deprecated

Function

# SecACLGetTypeID()

Returns the unique identifier of the opaque type to which an ACL entry belongs.

macOS 10.3–10.10Deprecated

``` source
func SecACLGetTypeID() -> CFTypeID
```

Deprecated

SecKeychain is deprecated

## Return Value

A value that identifies the opaque type of a SecACL object.

## Discussion

This function returns a value that uniquely identifies the opaque type of a SecACL instance. You can compare this value to the CFTypeID identifier obtained by calling the CFGetTypeID(_:) method on a specific instance. These values might change from release to release or platform to platform.

