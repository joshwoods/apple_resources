

- UIKit
- UIKey
-  charactersIgnoringModifiers 

Instance Property

# charactersIgnoringModifiers

A string that represents the text value of the key without modifier keys.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+tvOS 13.4+visionOS 1.0+

``` source
@MainActor
var charactersIgnoringModifiers: String { get }
```

## Mentioned in 

Handling key presses made on a physical keyboard

## Discussion

For Latin-based languages, always expect a lowercase property value. If the user is pressing only a modifier key, the property value is an empty string.

To check for special keys, compare charactersIgnoringModifiers to constants listed in Input strings for special keys.

## See Also

### Getting key characters

var characters: String

A string that represents the text value of the key combined with any active modifier keys.

