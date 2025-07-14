

- Foundation
-  AttributedSubstring 

Structure

# AttributedSubstring

A portion of an attributed string.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@dynamicMemberLookup
struct AttributedSubstring
```

## Overview

AttributedSubstring provides no-copy access to the contents of the string within the relevant range. The distinction between an AttributedString and an AttributedSubstring lets you distinguish between whether you’re in possession of an entire string or just a slice of it.

Because AttributedSubstring and AttributedString both conform to AttributedStringProtocol, working with ranges of AttributedString is natural. Modifying attributes by range works the same as it does on the base string.

If you use an AttributedSubstring to mutate its base AttributedString, you must perform your mutation inline, as the following example shows:

```
// Correct use of copying.
attrStr[range].link = url

// Incorrect use of AttributedString copy. Copies the referenced range of the base
// AttributedString and mutates that.
var substr = attrStr[range]
substr.link = url
```

## Topics

### Creating Attributed Substrings

init()

Creates an empty attributed substring.

### Applying and Modifying Attributes

enum AttributeMergePolicy

An enumeration of behaviors to apply when merging attributes.

### Accessing Indices

Accessing Indicies Within an Attributed Substring

### Accessing Views into the Attributed Substring

struct CharacterView

A view into the underlying storage of the attributed string, as Unicode characters.

struct UnicodeScalarView

A view into the underlying storage of the attributed string, as Unicode scalars.

struct Runs

An iterable view into segments of the attributed string, each of which indicates where a run of identical attributes begins or ends.

### Accessing the Underlying Attributed String

var base: AttributedString

Returns the underlying attributed string that the attributed substring derives from.

### Accessing Whole-Substring Attributes

enum AttributeDynamicLookup

A type to support dynamic member lookup of attributes and containers.

struct ScopedAttributeContainer

An attribute container that allows dynamic member lookup of its contents within the specified attribute scope.

## Relationships

### Conforms To

- AttributedStringAttributeMutation
- AttributedStringProtocol
- Copyable
- CustomStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Strings with Metadata

struct AttributedString

A value type for a string with associated attributes for portions of its text.

Attributed String Supporting Types

Types that the attributed string, attributed substring, and helper types extend or conform to, for sharing common functionality.

class NSAttributedString

A string of text that manages data, layout, and stylistic information for ranges of characters to support rendering.

class NSMutableAttributedString

A mutable string with associated attributes (such as visual style, hyperlinks, or accessibility data) for portions of its text.

