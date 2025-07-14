

- AVFoundation
- AVCaption
-  AVCaption.TextCombine 

Enumeration

# AVCaption.TextCombine

The caption’s supported rendering policy options.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
enum TextCombine
```

## Overview

Text combine is a special rendering policy that combines multiple characters into one unit and presents it in upright position in a vertical text flow. This presentation achieves a horizontal-in-vertical layout (or Tate-Chu-Yoko layout), which lets the caption render a horizontal text string in vertical text.

## Topics

### Text Combine Options

case all

An option that combines all of the characters.

case none

An option that doesn’t combine text upright.

case oneDigit

An option that makes one digit upright.

case twoDigits

An option that combines two consecutive digits.

case threeDigits

An option that combines three consecutive digits.

case fourDigits

An option that combines four consecutive digits.

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

### Accessing Advanced Typography

func ruby(at: String.Index) -> (AVCaption.Ruby?, Range&lt;String.Index>)

Returns the ruby text at the index position.

class Ruby

An object that presents ruby characters.

func textCombine(at: String.Index) -> (AVCaption.TextCombine, Range&lt;String.Index>)

Returns the text combine at the index position.

