

- Security
-  SecCodeGetTypeID() 

Function

# SecCodeGetTypeID()

Returns the unique identifier of the opaque type to which a code object belongs.

Mac Catalyst 13.0+macOS 10.0+

``` source
func SecCodeGetTypeID() -> CFTypeID
```

## Return Value

A value that identifies the opaque type of a code object.

## Discussion

You can compare the value returned by this function to the CFTypeID identifier obtained by calling the CFGetTypeID(_:) function on a specific object. These values might change from release to release or platform to platform.

