

- AppKit
-  NSChangeSpelling 

Protocol

# NSChangeSpelling

A protocol that responder objects can implement to correct a misspelled word.

macOS

``` source
protocol NSChangeSpelling
```

## Topics

### Changing spellings

func changeSpelling(Any?)

Replaces the selected word in the receiver with a corrected version from the Spelling panel.

**Required**

## Relationships

### Conforming Types

- NSText
- NSTextView

## See Also

### Spell-checking

class NSSpellChecker

An interface to the Cocoa spell-checking service.

protocol NSIgnoreMisspelledWords

A protocol that enables the Ignore button in the Spelling panel to function properly.

