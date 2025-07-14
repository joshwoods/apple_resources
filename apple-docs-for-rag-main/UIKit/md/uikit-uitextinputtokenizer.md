

- UIKit
-  UITextInputTokenizer 

Protocol

# UITextInputTokenizer

A tokenizer, which is an object that allows the text input system to evaluate text units of different granularities.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UITextInputTokenizer : NSObjectProtocol
```

## Overview

Granularities of text units are always evaluated with reference to a storage or reference direction.

Text-processing objects that conform to the UITextInput protocol must hold a reference to a tokenizer (through the tokenizer property). The UITextInputStringTokenizer class provides a default base implementation of the UITextInputTokenizer protocol. Tokenizers of this class are suitable for most western-language keyboards. Apps with different requirements may adopt the UITextInputTokenizer protocol and create their own tokenizers.

## Topics

### Determining text positions relative to unit boundaries

func isPosition(UITextPosition, atBoundary: UITextGranularity, inDirection: UITextDirection) -> Bool

Return whether a text position is at a boundary of a text unit of a specified granularity in a specified direction.

**Required**

func isPosition(UITextPosition, withinTextUnit: UITextGranularity, inDirection: UITextDirection) -> Bool

Return whether a text position is within a text unit of a specified granularity in a specified direction.

**Required**

### Computing text position by unit boundaries

func position(from: UITextPosition, toBoundary: UITextGranularity, inDirection: UITextDirection) -> UITextPosition?

Return the next text position at a boundary of a text unit of the given granularity in a given direction.

**Required**

### Getting ranges of specific text units

func rangeEnclosingPosition(UITextPosition, with: UITextGranularity, inDirection: UITextDirection) -> UITextRange?

Return the range for the text enclosing a text position in a text unit of a given granularity in a given direction.

**Required**

### Constants

struct UITextDirection

The direction of the text.

enum UITextGranularity

The granularity of a unit of text.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- UITextInputStringTokenizer

## See Also

### Text tokenizer

class UITextInputStringTokenizer

A base implementation of the text-input tokenizer protocol.

