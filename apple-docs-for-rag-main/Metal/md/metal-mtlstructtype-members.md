

- Metal
- MTLStructType
-  members 

Instance Property

# members

An array of objects that describe the fields in the struct.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var members: [MTLStructMember] { get }
```

## Discussion

Each array element in members is a MTLStructMember object that corresponds to one of the fields in the struct.

## See Also

### Related Documentation

Metal Shading Language Guide

Metal Programming Guide

### Obtaining Information about Struct Members

func memberByName(String) -> MTLStructMember?

Provides a representation of a struct member.

