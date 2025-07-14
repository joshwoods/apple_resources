

- Swift
- String
-  String.IntentInputOptions 

Structure

# String.IntentInputOptions

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct IntentInputOptions
```

## Topics

### Initializers

init(keyboardType: String.IntentInputOptions.KeyboardType, capitalizationType: String.IntentInputOptions.CapitalizationType, multiline: Bool, autocorrect: Bool, smartQuotes: Bool, smartDashes: Bool)

### Instance Properties

var autocorrect: Bool

var capitalizationType: String.IntentInputOptions.CapitalizationType

var keyboardType: String.IntentInputOptions.KeyboardType

var multiline: Bool

var smartDashes: Bool

var smartQuotes: Bool

### Enumerations

enum CapitalizationType

Describes the capitalization modes to apply to text.

enum KeyboardType

Describes the types of keyboard to use for text entry.

