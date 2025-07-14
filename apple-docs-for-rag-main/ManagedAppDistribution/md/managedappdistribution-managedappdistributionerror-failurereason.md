

- ManagedAppDistribution
- ManagedAppDistributionError
-  failureReason 

Instance Property

# failureReason

A detailed description of the error.

iOS 17.2+iPadOS 17.2+visionOS 2.4+

``` source
var failureReason: String? { get }
```

## Discussion

This appears in the body of an alert.

## See Also

### Providing error information

var description: String

A localized description of the error.

var errorDescription: String?

A brief description of the error.

var recoveryOptions: [String]

A set of possible recovery options to present.

var recoverySuggestion: String?

A suggestion for recovering from the error.

var localizedStringResource: LocalizedStringResource

A set of localized error strings.

