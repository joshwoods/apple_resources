

- Security
-  SecTaskGetTypeID() 

Function

# SecTaskGetTypeID()

Returns the unique identifier of the opaque type to which a task object belongs.

Mac Catalyst 13.0+macOS 10.0+

``` source
func SecTaskGetTypeID() -> CFTypeID
```

## Return Value

A value that identifies the opaque type of a SecTask object.

## Discussion

This function returns a value that uniquely identifies the opaque type of a SecTask object. You can compare this value to the CFTypeID identifier obtained by calling the CFGetTypeID(_:) function on a specific object. These values might change from release to release or platform to platform.

