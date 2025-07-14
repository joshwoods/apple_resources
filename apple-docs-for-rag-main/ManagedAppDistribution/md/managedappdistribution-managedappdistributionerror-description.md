

- ManagedAppDistribution
- ManagedAppDistributionError
-  description 

Instance Property

# description

A localized description of the error.

iOS 17.2+iPadOS 17.2+visionOS 2.4+

``` source
var description: String { get }
```

## See Also

### Providing error information

var errorDescription: String?

A brief description of the error.

var failureReason: String?

A detailed description of the error.

var recoveryOptions: [String]

A set of possible recovery options to present.

var recoverySuggestion: String?

A suggestion for recovering from the error.

var localizedStringResource: LocalizedStringResource

A set of localized error strings.

