

- App Intents
- IntentParameter
-  IntentParameter.InclusiveRange 

Type Alias

# IntentParameter.InclusiveRange

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
typealias InclusiveRange = (lowerBound: Bound, upperBound: Bound) where Bound : Comparable
```

Available when `Value` conforms to `_IntentValue` and `Sendable`.

## See Also

### Accessing the configuration

var currencyCodes: [String]?

var inclusiveRange: IntentParameter&lt;Value>.InclusiveRange&lt;Decimal>?

