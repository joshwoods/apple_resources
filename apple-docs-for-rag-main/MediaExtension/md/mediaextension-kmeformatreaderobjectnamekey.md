

- MediaExtension
-  kMEFormatReaderObjectNameKey 

Global Variable

# kMEFormatReaderObjectNameKey

A user-readable string describing the format reader.

Mac Catalyst 18.0+macOS 15.0+

``` source
var kMEFormatReaderObjectNameKey: String { get }
```

## Discussion

This string is used internally for uniquely identifying format readers and possibly for debug logging but is typically not visible to users.

## See Also

### Property list keys

var kMEFormatReaderClassImplementationIDKey: String

The unique identifier for the format reader.

var kMEFormatReaderExtensionPointName: String

A key to the extension point name for format readers.

var kMEFormatReaderFileNameExtensionArrayKey: String

A key to the array of file extensions that the format reader plug-in supports.

var kMEFormatReaderUTTypeArrayKey: String

A key to the array of Uniform Type Identifiers that the format reader supports.

