

- Local Authentication
- LAContext
-  maxBiometryFailures Deprecated

Instance Property

# maxBiometryFailures

The number of biometric authentication failures after which the context falls back to another mechanism.

iOS 8.3–9.0DeprecatediPadOS 8.3–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.10.3–10.11DeprecatedvisionOS 1.0–1.0Deprecated

``` source
var maxBiometryFailures: NSNumber? { get set }
```

Deprecated

Leave this value set to the default of `nil`, in which case authentication fails after 3 wrong attempts.

## Discussion

Biometry lockout happens after at most 5 wrong attempts, regardless of how you set this property.

## See Also

### Evaluating authentication policies

func evaluatePolicy(LAPolicy, localizedReason: String, reply: (Bool, (any Error)?) -> Void)

Evaluates the specified policy.

var evaluatedPolicyDomainState: Data?

The current state of the evaluated policy domain.

Deprecated

