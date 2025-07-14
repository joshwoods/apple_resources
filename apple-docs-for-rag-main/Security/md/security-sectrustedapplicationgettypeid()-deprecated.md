

- Security
-  SecTrustedApplicationGetTypeID() Deprecated

Function

# SecTrustedApplicationGetTypeID()

Returns the unique identifier of the opaque type to which a trusted app instance belongs.

macOS 10.2–10.10Deprecated

``` source
func SecTrustedApplicationGetTypeID() -> CFTypeID
```

Deprecated

SecKeychain is deprecated

## Return Value

A value that identifies the opaque type of a SecTrustedApplication object.

## Discussion

This function returns a value that uniquely identifies the opaque type of a SecTrustedApplication instance. You can compare this value to the CFTypeID identifier obtained by calling the CFGetTypeID(_:) method on a specific instance. These values might change from release to release or platform to platform.

