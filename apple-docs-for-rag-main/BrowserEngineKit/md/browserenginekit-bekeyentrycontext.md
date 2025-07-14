

- BrowserEngineKit
-  BEKeyEntryContext 

Class

# BEKeyEntryContext

A class that describes a key event and the text document with which the event is associated.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
class BEKeyEntryContext
```

## Overview

If the key entry occurs within the context of a composed input mode, for example Chinese, Japanese, or Korean input, set shouldEvaluateForInputSystemHandling to `true`. The text system uses the document’s marked text to combine multiple key events into a single input character.

## Topics

### Creating a key entry context

init(keyEntry: BEKeyEntry)

Initializes an instance of BEKeyEventContext with its corresponding `keyState`

### Getting the information about the key event

var keyEntry: BEKeyEntry

BEKeyEntry for which this context is representing.

var shouldInsertCharacter: Bool

Represents whether a character should be inserted.

var shouldEvaluateForInputSystemHandling: Bool

Represents whether the key event should be evaluated within the context of a composed input mode.

### Getting information about the text document

var isDocumentEditable: Bool

Represents whether the web document is editable

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

## See Also

### Keyboard input

class BEKeyEntry

A class that represents a keyboard event in the text system.

enum BEKeyModifierFlags

An enumeration that records the state of the shift-modifier keys.

