

- SwiftUI
-  TextInputDictationBehavior 

Structure

# TextInputDictationBehavior

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
struct TextInputDictationBehavior
```

## Topics

### Getting behavior values

static let automatic: TextInputDictationBehavior

A platform-appropriate default text input dictation behavior.

static func inline(activation: TextInputDictationActivation) -> TextInputDictationBehavior

Adds a dictation microphone in the search bar.

static let preventDictation: TextInputDictationBehavior

Prevents the search bar from having a dictation microphone.

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Dictating text

func searchDictationBehavior(TextInputDictationBehavior) -> some View

Configures the dictation behavior for any search fields configured by the searchable modifier.

struct TextInputDictationActivation

