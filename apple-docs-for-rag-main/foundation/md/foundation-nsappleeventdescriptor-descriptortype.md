

- Foundation
- NSAppleEventDescriptor
-  descriptorType 

Instance Property

# descriptorType

The descriptor type of the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
var descriptorType: DescType { get }
```

## See Also

### Getting Information About a Descriptor

var aeDesc: UnsafePointer&lt;AEDesc>?

The `AEDesc` structure encapsulated by the receiver, if it has one.

var booleanValue: Bool

The contents of the receiver as a Boolean value, coercing (to `typeBoolean`) if necessary.

func coerce(toDescriptorType: DescType) -> NSAppleEventDescriptor?

Returns a descriptor obtained by coercing the receiver to the specified type.

var data: Data

The receiver’s data.

var enumCodeValue: OSType

The contents of the receiver as an enumeration type, coercing to `typeEnumerated` if necessary.

var int32Value: Int32

The contents of the receiver as an integer, coercing (to `typeSInt32`) if necessary.

var numberOfItems: Int

The number of descriptors in the receiver’s descriptor list.

var stringValue: String?

The contents of the receiver as a Unicode text string, coercing to `typeUnicodeText` if necessary.

var typeCodeValue: OSType

The contents of the receiver as a type, coercing to `typeType` if necessary.

