

- Security
-  SecRequirementGetTypeID() 

Function

# SecRequirementGetTypeID()

Returns the unique identifier of the opaque type to which a code requirement object belongs.

Mac Catalyst 13.0+macOS 10.0+

``` source
func SecRequirementGetTypeID() -> CFTypeID
```

## Return Value

A value that identifies the opaque type of a SecRequirement object.

## Discussion

You can compare the value returned by this function to the CFTypeID identifier obtained by calling the CFGetTypeID(_:) function on a specific object. These values might change from release to release or platform to platform.

## See Also

### Related Documentation

func SecRequirementCreateWithString(CFString, SecCSFlags, UnsafeMutablePointer&lt;SecRequirement?>) -> OSStatus

Creates a code requirement object by compiling a valid text representation of a code requirement.

func SecRequirementCreateWithStringAndErrors(CFString, SecCSFlags, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?, UnsafeMutablePointer&lt;SecRequirement?>) -> OSStatus

Creates a code requirement object by compiling a valid text representation of a code requirement and returns detailed error information in the case of failure.

