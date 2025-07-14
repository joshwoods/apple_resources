

- App Intents
- IntentParameter
-  supportsNegativeNumbers 

Instance Property

# supportsNegativeNumbers

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
final var supportsNegativeNumbers: Bool? { get }
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, and `Value.ValueType` is `Measurement`.

## See Also

### Accessing unit details

var unit: IntentParameter&lt;Value>.Mass?

enum Mass

var defaultUnit: IntentParameter&lt;Value>.Mass?

var unitAdjustForLocale: Bool?

