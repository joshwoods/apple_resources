

- Metal
- MTLStructMember
-  dataType 

Instance Property

# dataType

The data type of the struct member.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var dataType: MTLDataType { get }
```

## Discussion

For information on possible values, see MTLDataType. If the value is MTLDataType.array, then the arrayType() method returns an object that describes the underlying array. If the value is MTLDataType.struct, then the structType() method returns an object that describes the underlying struct.

## See Also

### Describing the Struct Member

var name: String

The name of the struct member.

var offset: Int

The location of this member relative to the start of its struct, in bytes.

var argumentIndex: Int

The index in the argument table that corresponds to the struct member.

