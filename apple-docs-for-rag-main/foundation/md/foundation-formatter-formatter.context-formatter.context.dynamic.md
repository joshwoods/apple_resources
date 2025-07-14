

- Foundation
- Formatter
- Formatter.Context
-  Formatter.Context.dynamic 

Case

# Formatter.Context.dynamic

A formatting context determined automatically at runtime.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case dynamic
```

## Discussion

A Formatter.Context.dynamic context is automatically determined to be one of the following: Formatter.Context.standalone, Formatter.Context.beginningOfSentence, or Formatter.Context.middleOfSentence.

When used in combination with stringWithFormat:, the formatter returns a string proxy, formats the string using Formatter.Context.unknown, determines context based on the proxy string’s location, and then reformats the string accordingly.

## See Also

### Constants

case unknown

An unknown formatting context.

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

case standalone

The formatting context for stand-alone usage.

case listItem

The formatting context for a list or menu item.

case beginningOfSentence

The formatting context for the beginning of a sentence.

case middleOfSentence

The formatting context for the middle of a sentence.

