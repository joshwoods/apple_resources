

- Foundation
-  NSHFSTypeCodeFromFileType(\_:) 

Function

# NSHFSTypeCodeFromFileType(\_:)

Returns a file type code.

Mac Catalyst 13.0+macOS 10.0+

``` source
func NSHFSTypeCodeFromFileType(_ fileTypeString: String!) -> OSType
```

## Parameters 

`fileTypeString`  

A string of the sort encoded by `NSFileTypeForHFSTypeCode()`.

## Return Value

The HFS file type code corresponding to `fileTypeString`, or `0` if it cannot be found.

## See Also

### Working with HFS File Types

func NSFileTypeForHFSTypeCode(OSType) -> String!

Returns a string encoding a file type code.

func NSHFSTypeOfFile(String!) -> String!

Returns a string encoding a file type.

