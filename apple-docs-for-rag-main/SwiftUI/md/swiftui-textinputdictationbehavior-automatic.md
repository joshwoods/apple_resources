

- SwiftUI
- TextInputDictationBehavior
-  automatic 

Type Property

# automatic

A platform-appropriate default text input dictation behavior.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
static let automatic: TextInputDictationBehavior
```

## Discussion

The automatic behavior uses a TextInputDictationActivation value of onLook for visionOS apps and onSelect for iOS apps.

## See Also

### Getting behavior values

static func inline(activation: TextInputDictationActivation) -> TextInputDictationBehavior

Adds a dictation microphone in the search bar.

static let preventDictation: TextInputDictationBehavior

Prevents the search bar from having a dictation microphone.

