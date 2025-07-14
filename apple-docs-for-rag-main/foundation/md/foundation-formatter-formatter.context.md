

- Foundation
- Formatter
-  Formatter.Context 

Enumeration

# Formatter.Context

The formatting context for a formatter.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum Context
```

## Overview

Use formatting contexts to specify where the result of formatting will appear, so that the formatter can provide the most appropriate result.

For example, when formatting a date or date symbol for a French locale, you want the month name to be capitalized if it appears at the beginning of the sentence (“Juin est mon mois de naissance”), but not if it appears elsewhere (“Mon mois de naissance est juin”).

If the formatting context isn’t known ahead of time, specify Formatter.Context.dynamic to have the system determine the context automatically.

## Topics

### Constants

case unknown

An unknown formatting context.

case dynamic

A formatting context determined automatically at runtime.

case standalone

The formatting context for stand-alone usage.

case listItem

The formatting context for a list or menu item.

case beginningOfSentence

The formatting context for the beginning of a sentence.

case middleOfSentence

The formatting context for the middle of a sentence.

case unknown

An unknown formatting context.

case dynamic

A formatting context determined automatically at runtime.

case standalone

The formatting context for stand-alone usage.

case listItem

The formatting context for a list or menu item.

case beginningOfSentence

The formatting context for the beginning of a sentence.

case middleOfSentence

The formatting context for the middle of a sentence.

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

### Constants

enum UnitStyle

Specifies the width of the unit, determining the textual representation.

