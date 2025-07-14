

- UIKit
-  UITextInputStringTokenizer 

Class

# UITextInputStringTokenizer

A base implementation of the text-input tokenizer protocol.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UITextInputStringTokenizer
```

## Overview

If you want to take advantage of this base implementation of the UITextInputTokenizer protocol, you should subclass this class and handle application-specific directions and granularities affected by layout. When you instantiate a class you must supply the document class that’s adopting the UITextInput protocol for your application.

### Subclassing notes

When you subclass UITextInputStringTokenizer, override all UITextInputTokenizer methods, calling the superclass implementation (`super`) when method parameters aren’t affected by layout. For example, the subclass needs a custom implementation of all methods for line granularity. For the left direction, it needs to decide whether left corresponds at a given position to forward or backward, and then call `super` passing in the storage direction (UITextStorageDirection).

## Topics

### Initializing a tokenizer

init(textInput: any UIResponder &amp; UITextInput)

Returns an object initialized with the document object that directly communicates with the text input system.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable
- UITextInputTokenizer

## See Also

### Text tokenizer

protocol UITextInputTokenizer

A tokenizer, which is an object that allows the text input system to evaluate text units of different granularities.

