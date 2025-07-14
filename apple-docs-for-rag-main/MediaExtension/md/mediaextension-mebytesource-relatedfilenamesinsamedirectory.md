

- MediaExtension
- MEByteSource
-  relatedFileNamesInSameDirectory 

Instance Property

# relatedFileNamesInSameDirectory

An array of related file names in the parent directory of the byte source file.

macOS 14.0+

``` source
var relatedFileNamesInSameDirectory: [String] { get }
```

## Discussion

The array of related files within the MEByteSource’s parent directory that are accessible to the MEByteSource. Only the relative file names are returned, not the paths. Only files with file extensions listed in the kMEFormatReaderFileNameExtensionArrayKey array in the format reader property list will be returned. If no related files are available, returns an empty array.

## See Also

### Inspecting a byte source

var fileName: String

The name of the file for the byte source.

var fileLength: Int64

The length of the byte source file.

var contentType: UTType?

The format of the byte source file.

