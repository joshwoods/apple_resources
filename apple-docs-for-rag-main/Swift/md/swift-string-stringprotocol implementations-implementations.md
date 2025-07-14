

- Swift
- String
-  StringProtocol Implementations 

API Collection

# StringProtocol Implementations

## Topics

### Structures

struct UTF16View

A view of a string’s contents as a collection of UTF-16 code units.

struct UTF8View

A view of a string’s contents as a collection of UTF-8 code units.

struct UnicodeScalarView

A view of a string’s contents as a collection of Unicode scalar values.

### Operators

static func != &lt;RHS>(Self, RHS) -> Bool

static func == &lt;RHS>(Self, RHS) -> Bool

static func > &lt;RHS>(Self, RHS) -> Bool

static func &lt; &lt;RHS>(Self, RHS) -> Bool

static func &lt;= &lt;RHS>(Self, RHS) -> Bool

static func >= &lt;RHS>(Self, RHS) -> Bool

### Initializers

init(cString: UnsafePointer&lt;CChar>)

Creates a new string by copying the null-terminated UTF-8 data referenced by the given pointer.

init&lt;C, Encoding>(decoding: C, as: Encoding.Type)

Creates a string from the given Unicode code units in the specified encoding.

init&lt;Encoding>(decodingCString: UnsafePointer&lt;Encoding.CodeUnit>, as: Encoding.Type)

Creates a new string by copying the null-terminated sequence of code units referenced by the given pointer.

### Instance Properties

var unicodeScalars: String.UnicodeScalarView

The string’s value represented as a collection of Unicode scalar values.

var utf16: String.UTF16View

A UTF-16 encoding of `self`.

var utf8: String.UTF8View

A UTF-8 encoding of `self`.

### Instance Methods

func hasPrefix(String) -> Bool

func hasSuffix(String) -> Bool

func lowercased() -> String

Returns a lowercase version of the string.

func uppercased() -> String

Returns an uppercase version of the string.

func withCString&lt;Result>((UnsafePointer&lt;Int8>) throws -> Result) rethrows -> Result

Calls the given closure with a pointer to the contents of the string, represented as a null-terminated sequence of UTF-8 code units.

func withCString&lt;Result, TargetEncoding>(encodedAs: TargetEncoding.Type, (UnsafePointer&lt;TargetEncoding.CodeUnit>) throws -> Result) rethrows -> Result

Calls the given closure with a pointer to the contents of the string, represented as a null-terminated sequence of code units.

