

- MediaExtension
- MEByteSource
-  fileName 

Instance Property

# fileName

The name of the file for the byte source.

macOS 14.0+

``` source
var fileName: String { get }
```

## See Also

### Inspecting a byte source

var fileLength: Int64

The length of the byte source file.

var contentType: UTType?

The format of the byte source file.

var relatedFileNamesInSameDirectory: [String]

An array of related file names in the parent directory of the byte source file.

