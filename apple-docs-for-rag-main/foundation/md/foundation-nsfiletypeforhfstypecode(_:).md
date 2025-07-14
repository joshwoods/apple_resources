

- Foundation
-  NSFileTypeForHFSTypeCode(\_:) 

Function

# NSFileTypeForHFSTypeCode(\_:)

Returns a string encoding a file type code.

Mac Catalyst 13.0+macOS 10.0+

``` source
func NSFileTypeForHFSTypeCode(_ hfsFileTypeCode: OSType) -> String!
```

## Parameters 

`hfsFileTypeCode`  

An HFS file type code.

## Return Value

A string that encodes `hfsFileTypeCode`.

## See Also

### Working with HFS File Types

func NSHFSTypeCodeFromFileType(String!) -> OSType

Returns a file type code.

func NSHFSTypeOfFile(String!) -> String!

Returns a string encoding a file type.

