

- App Intents
- IntentParameter
-  currencyCodes 

Instance Property

# currencyCodes

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
final var currencyCodes: [String]? { get }
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, and `Value.ValueType` is `IntentCurrencyAmount`.

## See Also

### Accessing the configuration

var inclusiveRange: IntentParameter&lt;Value>.InclusiveRange&lt;Decimal>?

typealias InclusiveRange

