

- App Intents
- IntentParameter
-  unit 

Instance Property

# unit

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
final var unit: IntentParameter.ElectricPotentialDifference? { get }
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, and `Value.ValueType` is `Measurement`.

## See Also

### Accessing unit details

enum ElectricPotentialDifference

var defaultUnit: IntentParameter&lt;Value>.ElectricPotentialDifference?

var supportsNegativeNumbers: Bool?

var unitAdjustForLocale: Bool?

