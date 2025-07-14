

- Swift
- String
-  String.Index 

Structure

# String.Index

A position of a character or code unit in a string.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct Index
```

## Topics

### Initializers

init?(String.Index, within: String.UTF16View)

Creates an index in the given UTF-16 view that corresponds exactly to the specified string position.

init?(String.Index, within: String)

Creates an index in the given string that corresponds exactly to the specified position.

init?&lt;S>(AttributedString.Index, within: S)

init?&lt;S>(String.Index, within: S)

Creates an index in the given string that corresponds exactly to the specified position.

init?(String.Index, within: String.UTF8View)

Creates an index in the given UTF-8 view that corresponds exactly to the specified `UTF16View` position.

init?(String.Index, within: String.UnicodeScalarView)

Creates an index in the given Unicode scalars view that corresponds exactly to the specified `UTF16View` position.

init(encodedOffset: Int)

Creates a new index at the specified code unit offset.

init&lt;S>(utf16Offset: Int, in: S)

Creates a new index at the specified UTF-16 code unit offset

### Instance Properties

var encodedOffset: Int

The offset into a string’s code units for this index.

### Instance Methods

func samePosition(in: String.UTF8View) -> String.UTF8View.Index?

Returns the position in the given UTF-8 view that corresponds exactly to this index.

func samePosition(in: String.UnicodeScalarView) -> String.UnicodeScalarIndex?

Returns the position in the given view of Unicode scalars that corresponds exactly to this index.

func samePosition(in: String) -> String.Index?

Returns the position in the given string that corresponds exactly to this index.

func samePosition(in: String.UTF16View) -> String.UTF16View.Index?

Returns the position in the given UTF-16 view that corresponds exactly to this index.

func utf16Offset&lt;S>(in: S) -> Int

The UTF-16 code unit offset corresponding to this index.

### Default Implementations

Comparable Implementations

CustomDebugStringConvertible Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Comparable
- Copyable
- CustomDebugStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Related String Types

struct Substring

A slice of a string.

protocol StringProtocol

A type that can represent a string as a collection of characters.

struct UnicodeScalarView

A view of a string’s contents as a collection of Unicode scalar values.

struct UTF16View

A view of a string’s contents as a collection of UTF-16 code units.

struct UTF8View

A view of a string’s contents as a collection of UTF-8 code units.

struct Iterator

A type that provides the collection’s iteration interface and encapsulates its iteration state.

struct Encoding

