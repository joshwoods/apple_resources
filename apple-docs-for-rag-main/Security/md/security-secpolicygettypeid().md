

- Security
-  SecPolicyGetTypeID() 

Function

# SecPolicyGetTypeID()

Returns the unique identifier of the opaque type to which a policy object belongs.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.3+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func SecPolicyGetTypeID() -> CFTypeID
```

## Return Value

A value that identifies the opaque type of a SecPolicy object.

## Discussion

This function returns a value that uniquely identifies the opaque type of a SecPolicy object. You can compare this value to the CFTypeID identifier obtained by calling the CFGetTypeID(_:) function on a specific object. These values might change from release to release or platform to platform.

