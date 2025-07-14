

- Core Foundation
- CFPropertyList
-  Reading and Writing Error Codes 

API Collection

# Reading and Writing Error Codes

Error codes for property list reading and writing functions such as CFPropertyListCreateWithData(_:_:_:_:_:).

## Topics

### Constants

var kCFPropertyListReadCorruptError: CFIndex

Signifies an error parsing a property list.

var kCFPropertyListReadUnknownVersionError: CFIndex

Signifies the version number in the property list is unknown.

var kCFPropertyListReadStreamError: CFIndex

Signifies a stream error reading a property list.

var kCFPropertyListWriteStreamError: CFIndex

Signifies a stream error writing a property list.

## See Also

### Constants

enum CFPropertyListFormat

Specifies the format of a property list.

Property List Mutability Options

Option flags that determine the degree of mutability of newly created property lists.

