

- App Intents
- IntentParameter
-  supportsNegativeNumbers 

Instance Property

# supportsNegativeNumbers

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
final var supportsNegativeNumbers: Bool? { get }
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, and `Value.ValueType` is `Measurement`.

## See Also

### Accessing unit details

var unit: IntentParameter&lt;Value>.Angle?

enum Angle

var defaultUnit: IntentParameter&lt;Value>.Angle?

var unitAdjustForLocale: Bool?

