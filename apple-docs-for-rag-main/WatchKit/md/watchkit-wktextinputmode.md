

- WatchKit
-  WKTextInputMode 

Enumeration

# WKTextInputMode

The input modes supported by the text input controller.

watchOS

``` source
enum WKTextInputMode
```

## Topics

### Constants

case plain

Text from dictation and suggestions only. Do not allow emoji of any kind.

case allowEmoji

Text from dictation and suggestions plus non animated emoji.

case allowAnimatedEmoji

Text from dictation and suggestions plus both animated and non animated emoji.

Deprecated

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

### Handling text input

func presentTextInputController(withSuggestions: [String]?, allowedInputMode: WKTextInputMode, completion: ([Any]?) -> Void)

Displays a modal interface for gathering text input from the user.

func presentTextInputControllerWithSuggestions(forLanguage: ((String) -> [Any]?)?, allowedInputMode: WKTextInputMode, completion: ([Any]?) -> Void)

Displays a modal interface for gathering language-specific text input from the user.

func dismissTextInputController()

Dismisses the text input controller without returning any text.

