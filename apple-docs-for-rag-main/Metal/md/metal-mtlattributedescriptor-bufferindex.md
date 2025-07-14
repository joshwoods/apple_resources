

- Metal
- MTLAttributeDescriptor
-  bufferIndex 

Instance Property

# bufferIndex

The index in the buffer argument table for the buffer that contains the data for this attribute.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var bufferIndex: Int { get set }
```

## See Also

### Defining Attribute Location

var offset: Int

The offset, in bytes, from the start of the buffer containing the attribute data to the start of the data itself.

var format: MTLAttributeFormat

The format of the attribute’s data.

enum MTLAttributeFormat

Values indicating the organization and format of data for function attributes.

