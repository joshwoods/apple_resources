

- Core Text
-  CTFontCollectionCopyOptions 

Structure

# CTFontCollectionCopyOptions

Option bits for use with CTFontCollectionCopyFontAttribute(s).

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.7+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
struct CTFontCollectionCopyOptions
```

## Topics

### Constants

static var standardSort: CTFontCollectionCopyOptions

Passing this option indicates that the return values should be sorted in standard UI order, suitable for display to the user. This is the same sorting behavior used by `NSFontPanel` and Font Book.

static var unique: CTFontCollectionCopyOptions

Passing this option indicates that duplicate values should be removed from the results.

### Initializers

init(rawValue: UInt32)

Creates a copy options structure with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Constants

let kCTFontCollectionRemoveDuplicatesOption: CFString

