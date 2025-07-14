

- App Intents
- IntentParameter
-  unit 

Instance Property

# unit

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
final var unit: IntentParameter.Energy? { get }
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, and `Value.ValueType` is `Measurement`.

## See Also

### Accessing unit details

enum Energy

var defaultUnit: IntentParameter&lt;Value>.Energy?

var supportsNegativeNumbers: Bool?

var unitAdjustForLocale: Bool?

