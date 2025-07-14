

- MediaExtension
- MEFormatReaderExtension
-  formatReader(with:options:) 

Instance Method

# formatReader(with:options:)

Creates a new format reader with the byte source and options that you specify.

macOS 14.0+

``` source
func formatReader(
    with primaryByteSource: MEByteSource,
    options: MEFormatReaderInstantiationOptions?
) throws -> any MEFormatReader
```

**Required**

## Parameters 

`primaryByteSource`  

The primary byte source for the format reader.

`options`  

The reader instantiation options.

## Return Value

A new format reader.

## See Also

### Creating a format reader

init()

Creates a new format reader factory.

**Required**

