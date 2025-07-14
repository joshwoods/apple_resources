

- Foundation
-  NSHFSTypeOfFile(\_:) 

Function

# NSHFSTypeOfFile(\_:)

Returns a string encoding a file type.

Mac Catalyst 13.0+macOS 10.0+

``` source
func NSHFSTypeOfFile(_ fullFilePath: String!) -> String!
```

## Parameters 

`fullFilePath`  

The full absolute path of a file.

## Return Value

A string that encodes `fullFilePath`’s HFS file type, or `nil` if the operation was not successful

## See Also

### Working with HFS File Types

func NSFileTypeForHFSTypeCode(OSType) -> String!

Returns a string encoding a file type code.

func NSHFSTypeCodeFromFileType(String!) -> OSType

Returns a file type code.

