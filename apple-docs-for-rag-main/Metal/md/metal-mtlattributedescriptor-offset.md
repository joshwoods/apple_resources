

- Metal
- MTLAttributeDescriptor
-  offset 

Instance Property

# offset

The offset, in bytes, from the start of the buffer containing the attribute data to the start of the data itself.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var offset: Int { get set }
```

## See Also

### Defining Attribute Location

var bufferIndex: Int

The index in the buffer argument table for the buffer that contains the data for this attribute.

var format: MTLAttributeFormat

The format of the attribute’s data.

enum MTLAttributeFormat

Values indicating the organization and format of data for function attributes.

