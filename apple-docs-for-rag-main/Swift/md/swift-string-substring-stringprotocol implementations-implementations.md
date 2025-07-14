

- Swift
- String
- Substring
-  StringProtocol Implementations 

API Collection

# StringProtocol Implementations

## Topics

### Structures

struct UTF16View

struct UTF8View

struct UnicodeScalarView

### Operators

static func != &lt;RHS>(Self, RHS) -> Bool

static func == &lt;RHS>(Self, RHS) -> Bool

static func > &lt;RHS>(Self, RHS) -> Bool

static func &lt; &lt;RHS>(Self, RHS) -> Bool

static func &lt;= &lt;RHS>(Self, RHS) -> Bool

static func >= &lt;RHS>(Self, RHS) -> Bool

### Initializers

init(cString: UnsafePointer&lt;CChar>)

Creates a string from the null-terminated, UTF-8 encoded sequence of bytes at the given pointer.

init&lt;C, Encoding>(decoding: C, as: Encoding.Type)

Creates a string from the given Unicode code units in the specified encoding.

init&lt;Encoding>(decodingCString: UnsafePointer&lt;Encoding.CodeUnit>, as: Encoding.Type)

Creates a string from the null-terminated sequence of bytes at the given pointer.

### Instance Properties

var unicodeScalars: Substring.UnicodeScalarView

var utf16: Substring.UTF16View

var utf8: Substring.UTF8View

### Instance Methods

func hasPrefix&lt;Prefix>(Prefix) -> Bool

Returns a Boolean value indicating whether the string begins with the specified prefix.

func hasSuffix&lt;Suffix>(Suffix) -> Bool

Returns a Boolean value indicating whether the string ends with the specified suffix.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

func lowercased() -> String

func uppercased() -> String

func withCString&lt;Result>((UnsafePointer&lt;CChar>) throws -> Result) rethrows -> Result

Calls the given closure with a pointer to the contents of the string, represented as a null-terminated sequence of UTF-8 code units.

func withCString&lt;Result, TargetEncoding>(encodedAs: TargetEncoding.Type, (UnsafePointer&lt;TargetEncoding.CodeUnit>) throws -> Result) rethrows -> Result

Calls the given closure with a pointer to the contents of the string, represented as a null-terminated sequence of code units.

