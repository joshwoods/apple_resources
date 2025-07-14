

- Natural Language
-  NLTokenUnit 

Enumeration

# NLTokenUnit

Constants representing linguistic units.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
enum NLTokenUnit
```

## Overview

You use these constants with these methods:

- availableTagSchemes(for:language:)

- tagsInRange:unit:scheme:options:tokenRanges:

- enumerateTagsInRange:unit:scheme:options:usingBlock:

## Topics

### Constants

case word

An individual word.

case sentence

An individual sentence.

case paragraph

An individual paragraph.

case document

The document in its entirety.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Determining the range of a unit token

func tokenRange(at: String.Index, unit: NLTokenUnit) -> Range&lt;String.Index>

Returns the range of the linguistic unit containing the specified character index.

func tokenRange(for: Range&lt;String.Index>, unit: NLTokenUnit) -> Range&lt;String.Index>

Finds the entire range of all tokens of the specified linguistic unit contained completely or partially within the specified range.

