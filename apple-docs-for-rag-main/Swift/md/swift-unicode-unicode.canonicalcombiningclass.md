

- Swift
- Unicode
-  Unicode.CanonicalCombiningClass 

Structure

# Unicode.CanonicalCombiningClass

The classification of a scalar used in the Canonical Ordering Algorithm defined by the Unicode Standard.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct CanonicalCombiningClass
```

## Overview

Canonical combining classes are used by the ordering algorithm to determine if two sequences of combining marks should be considered canonically equivalent (that is, identical in interpretation). Two sequences are canonically equivalent if they are equal when sorting the scalars in ascending order by their combining class.

For example, consider the sequence `"\u{0041}\u{0301}\u{0316}"` (LATIN CAPITAL LETTER A, COMBINING ACUTE ACCENT, COMBINING GRAVE ACCENT BELOW). The combining classes of these scalars have the numeric values 0, 230, and 220, respectively. Sorting these scalars by their combining classes yields `"\u{0041}\u{0316}\u{0301}"`, so two strings that differ only by the ordering of those scalars would compare as equal:

```
let aboveBeforeBelow = "\u{0041}\u{0301}\u{0316}"
let belowBeforeAbove = "\u{0041}\u{0316}\u{0301}"
print(aboveBeforeBelow == belowBeforeAbove)
// Prints "true"
```

# Named and Unnamed Combining Classes

Canonical combining classes are defined in the Unicode Standard as integers in the range `0...254`. For convenience, the standard assigns symbolic names to a subset of these combining classes.

The `CanonicalCombiningClass` type conforms to `RawRepresentable` with a raw value of type `UInt8`. You can create instances of the type by using the static members named after the symbolic names, or by using the `init(rawValue:)` initializer.

```
let overlayClass = Unicode.CanonicalCombiningClass(rawValue: 1)
let overlayClassIsOverlay = overlayClass == .overlay
// overlayClassIsOverlay == true
```

## Topics

### Operators

static func == (Unicode.CanonicalCombiningClass, Unicode.CanonicalCombiningClass) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func &lt; (Unicode.CanonicalCombiningClass, Unicode.CanonicalCombiningClass) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than that of the second argument.

### Initializers

init(rawValue: UInt8)

Creates a new canonical combining class with the given raw integer value.

### Instance Properties

var hashValue: Int

The hash value.

let rawValue: UInt8

The raw integer value of the canonical combining class.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static let above: Unicode.CanonicalCombiningClass

Distinct marks directly above.

static let aboveLeft: Unicode.CanonicalCombiningClass

Distinct marks at the top left.

static let aboveRight: Unicode.CanonicalCombiningClass

Distinct marks at the top right.

static let attachedAbove: Unicode.CanonicalCombiningClass

Marks attached directly above.

static let attachedAboveRight: Unicode.CanonicalCombiningClass

Marks attached at the top right.

static let attachedBelow: Unicode.CanonicalCombiningClass

Marks attached directly below.

static let attachedBelowLeft: Unicode.CanonicalCombiningClass

Marks attached at the bottom left.

static let below: Unicode.CanonicalCombiningClass

Distinct marks directly below.

static let belowLeft: Unicode.CanonicalCombiningClass

Distinct marks at the bottom left.

static let belowRight: Unicode.CanonicalCombiningClass

Distinct marks at the bottom right.

static let doubleAbove: Unicode.CanonicalCombiningClass

Distinct marks extending above two bases.

static let doubleBelow: Unicode.CanonicalCombiningClass

Distinct marks subtending two bases.

static let iotaSubscript: Unicode.CanonicalCombiningClass

Greek iota subscript only (U+0345 COMBINING GREEK YPOGEGRAMMENI).

static let kanaVoicing: Unicode.CanonicalCombiningClass

Combining marks that are attached to hiragana and katakana to indicate voicing changes.

static let left: Unicode.CanonicalCombiningClass

Distinct marks to the left.

static let notReordered: Unicode.CanonicalCombiningClass

Base glyphs that occupy their own space and do not combine with others.

static let nukta: Unicode.CanonicalCombiningClass

Diacritic nukta marks in Brahmi-derived scripts.

static let overlay: Unicode.CanonicalCombiningClass

Marks that overlay a base letter or symbol.

static let right: Unicode.CanonicalCombiningClass

Distinct marks to the right.

static let virama: Unicode.CanonicalCombiningClass

Diacritic virama marks in Brahmi-derived scripts.

### Default Implementations

Comparable Implementations

Equatable Implementations

## Relationships

### Conforms To

- Comparable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Unicode Scalar Classifications

enum GeneralCategory

The most general classification of a Unicode scalar.

enum NumericType

The numeric type of a scalar.

