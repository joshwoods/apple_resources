

- Core Foundation
-  CFStringCompareFlags 

Structure

# CFStringCompareFlags

A CFOptionFlags type for specifying options for string comparison .

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CFStringCompareFlags
```

## Overview

See String Comparison Flags for values.

## Topics

### Initializers

init(rawValue: CFOptionFlags)

### Type Properties

static var compareAnchored: CFStringCompareFlags

Performs searching only on characters at the beginning or end of the range.

static var compareBackwards: CFStringCompareFlags

Specifies that the comparison should start at the last elements of the entities being compared (for example, strings or arrays).

static var compareCaseInsensitive: CFStringCompareFlags

Specifies that the comparison should ignore differences in case between alphabetical characters.

static var compareDiacriticInsensitive: CFStringCompareFlags

Specifies that the comparison should ignore diacritic markers.

static var compareForcedOrdering: CFStringCompareFlags

Specifies that the comparison is forced to return either `kCFCompareLessThan` or `kCFCompareGreaterThan` if the strings are equivalent but not strictly equal.

static var compareLocalized: CFStringCompareFlags

Specifies that the comparison should take into account differences related to locale, such as the thousands separator character.

static var compareNonliteral: CFStringCompareFlags

Specifies that loose equivalence is acceptable, especially as pertains to diacritical marks.

static var compareNumerically: CFStringCompareFlags

Specifies that represented numeric values should be used as the basis for comparison and not the actual character values.

static var compareWidthInsensitive: CFStringCompareFlags

Specifies that the comparison should ignore width differences.

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

### Data Types

typealias CFStringEncoding

An integer type for constants used to specify supported string encodings in various CFString functions.

enum CFStringEncodings

Index type for constants used to specify external string encodings.

struct CFStringInlineBuffer

Defines the buffer and related fields used for in-line buffer access of characters in CFString objects.

