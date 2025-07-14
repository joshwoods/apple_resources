

- SwiftUI
-  TextInputDictationActivation 

Structure

# TextInputDictationActivation

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
struct TextInputDictationActivation
```

## Topics

### Getting activation values

static let onLook: TextInputDictationActivation

A configuration that activates dictation when someone selects the microphone or looks at the entry field.

static let onSelect: TextInputDictationActivation

A configuration that activates dictation when someone selects the microphone.

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Dictating text

func searchDictationBehavior(TextInputDictationBehavior) -> some View

Configures the dictation behavior for any search fields configured by the searchable modifier.

struct TextInputDictationBehavior

