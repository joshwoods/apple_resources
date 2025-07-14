

- AppKit
- NSTextList
-  NSTextList.MarkerFormat 

Structure

# NSTextList.MarkerFormat

Constants that describe marker symbols you can apply to list elements in text lists.

macOS 10.0+

``` source
struct MarkerFormat
```

## Overview

Select a marker symbol to apply to your list elements in your text list, then set it in markerFormat. Or, specify a marker symbol when you create a text list with init(markerFormat:options:) or init(markerFormat:options:startingItemNumber:).

## Topics

### Selecting a marker format

static let box: NSTextList.MarkerFormat

The value that represents a square-shaped marker that you can apply to a text list item.

static let check: NSTextList.MarkerFormat

The value that represents a checkmark-shaped marker that you can apply to a text list item.

static let circle: NSTextList.MarkerFormat

The value that represents a circle-shaped marker that you can apply to a text list item.

static let decimal: NSTextList.MarkerFormat

The value that represents a decimal annotation marker that you can apply to a text list item.

static let diamond: NSTextList.MarkerFormat

The value that represents a diamond-shaped marker that you can apply to a text list item.

static let disc: NSTextList.MarkerFormat

The value that represents a disc-shaped marker that you can apply to a text list item.

static let hyphen: NSTextList.MarkerFormat

The value that represents a hyphen-shaped marker that you can apply to a text list item.

static let lowercaseAlpha: NSTextList.MarkerFormat

The value that represents a lowercase localized alphabetical marker you that can apply to a text list item.

static let lowercaseHexadecimal: NSTextList.MarkerFormat

The value that represents a lowercase hexadecimal (base 16) numerical marker that you can apply to a text list item.

static let lowercaseLatin: NSTextList.MarkerFormat

The value that represents a lowercase Latin alphabetical marker that you can apply to a text list item.

static let lowercaseRoman: NSTextList.MarkerFormat

The value that represents a lowercase Roman numeral marker that you can apply to a text list item.

static let octal: NSTextList.MarkerFormat

The value that represents an octal (base 8) numerical marker that you can apply to a text list item.

static let square: NSTextList.MarkerFormat

The value that represents a square-shaped marker that you can apply to a text list item.

static let uppercaseAlpha: NSTextList.MarkerFormat

The value that represents an uppercase localized alphabetical marker that you can apply to a text list item.

static let uppercaseHexadecimal: NSTextList.MarkerFormat

The value that represents an uppercase hexadecimal (base 16) numerical marker that you can apply to a text list item.

static let uppercaseLatin: NSTextList.MarkerFormat

The value that represents an uppercase Latin alphabetical marker that you can apply to a text list item.

static let uppercaseRoman: NSTextList.MarkerFormat

The value that represents an uppercase Roman numeral marker that you can apply to a text list item.

### Initializing a marker format

init(String)

Creates a new marker that you can apply to an item in a text list with the raw value you provide.

init(rawValue: String)

Creates a new marker that you can apply to an item in a text list using the string you provide.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Working with markers

var markerFormat: NSTextList.MarkerFormat

Returns the marker format string used by the receiver.

func marker(forItemNumber: Int) -> String

Returns the computed value for a specific ordinal position in the list.

