

- Local Authentication
- LAPolicy
-  LAPolicy.deviceOwnerAuthenticationWithBiometricsOrWatch Deprecated

Case

# LAPolicy.deviceOwnerAuthenticationWithBiometricsOrWatch

User authentication with either biometry or Apple Watch.

macOS 10.15–15.0Deprecated

``` source
case deviceOwnerAuthenticationWithBiometricsOrWatch
```

## Discussion

You use the LAPolicy.deviceOwnerAuthenticationWithBiometricsOrWatch policy when calling the evaluatePolicy(_:localizedReason:reply:) method to authenticate the user with either Apple Watch or biometrics. The authentication mechanisms run in parallel until one or the other succeeds, or until the user cancels the operation.

If the evaluation method can’t find a nearby, paired Apple Watch running watchOS 6 or later, this policy reverts to the behavior of the LAPolicy.deviceOwnerAuthenticationWithBiometrics policy. If biometry is unavailable, the policy behaves like the LAPolicy.deviceOwnerAuthenticationWithWatch policy.

To allow the user to authenticate with either of these options or a password, use the LAPolicy.deviceOwnerAuthentication policy instead.

## See Also

### Policies

case deviceOwnerAuthenticationWithBiometrics

User authentication with biometry.

case deviceOwnerAuthenticationWithWatch

User authentication with Apple Watch.

Deprecated

case deviceOwnerAuthentication

User authentication with biometry, Apple Watch, or the device passcode.

case deviceOwnerAuthenticationWithWristDetection

User authentication with wrist detection on watchOS.

