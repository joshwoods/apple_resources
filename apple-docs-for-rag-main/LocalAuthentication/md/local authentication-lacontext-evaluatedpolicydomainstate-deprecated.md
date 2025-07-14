

- Local Authentication
- LAContext
-  evaluatedPolicyDomainState Deprecated

Instance Property

# evaluatedPolicyDomainState

The current state of the evaluated policy domain.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var evaluatedPolicyDomainState: Data? { get }
```

## Discussion

The value of this property is non-`nil` when the canEvaluatePolicy(_:error:) method succeeds for a biometric policy or the person successfully authenticates using biometrics, following a call to evaluatePolicy(_:localizedReason:reply:). Otherwise, its value is `nil`.

Compare the values you get from successive calls to this property to determine whether the authorized database changed. However, the value you get doesn’t describe the nature of a change; it only lets you detect if a change happens.

Note

The value of this property is different in different processes, so you can’t compare the value from one app to the value from another app.

## See Also

### Evaluating authentication policies

func evaluatePolicy(LAPolicy, localizedReason: String, reply: (Bool, (any Error)?) -> Void)

Evaluates the specified policy.

var maxBiometryFailures: NSNumber?

The number of biometric authentication failures after which the context falls back to another mechanism.

Deprecated

