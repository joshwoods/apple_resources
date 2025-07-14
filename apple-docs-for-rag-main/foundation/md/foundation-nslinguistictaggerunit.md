

- Foundation
-  NSLinguisticTaggerUnit 

Enumeration

# NSLinguisticTaggerUnit

Constants representing linguistic units.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum NSLinguisticTaggerUnit
```

## Overview

You use these constants with the availableTagSchemes(for:language:) method as well as the tag(for:at:unit:scheme:orthography:tokenRange:), tags(in:unit:scheme:options:tokenRanges:), and enumerateTags(in:unit:scheme:options:using:) methods.

## Topics

### Constants

case document

The document in its entirety.

case paragraph

An individual paragraph.

case sentence

An individual sentence.

case word

An individual word.

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

### Supporting Types

struct NSLinguisticTagScheme

Constants for the tag schemes specified when initializing a linguistic tagger.

struct NSLinguisticTag

A token, lexical class, name, lemma, language, or script returned by a linguistic tagger for natural language text.

