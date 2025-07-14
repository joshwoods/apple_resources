

- Foundation
-  NSBinarySearchingOptions 

Structure

# NSBinarySearchingOptions

Options for searches and insertions using index(of:inSortedRange:options:usingComparator:).

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct NSBinarySearchingOptions
```

## Topics

### Constants

static var firstEqual: NSBinarySearchingOptions

Specifies that the search should return the first object in the range that is equal to the given object.

static var lastEqual: NSBinarySearchingOptions

Specifies that the search should return the last object in the range that is equal to the given object.

static var insertionIndex: NSBinarySearchingOptions

Returns the index at which you should insert the object in order to maintain a sorted array.

### Initializers

init(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

