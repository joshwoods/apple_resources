

- Local Authentication
- LAPolicy
-  LAPolicy.deviceOwnerAuthenticationWithWatch Deprecated

Case

# LAPolicy.deviceOwnerAuthenticationWithWatch

User authentication with Apple Watch.

macOS 10.15–15.0Deprecated

``` source
case deviceOwnerAuthenticationWithWatch
```

## Discussion

You use the LAPolicy.deviceOwnerAuthenticationWithWatch policy when calling the evaluatePolicy(_:localizedReason:reply:) method to authenticate the user with Apple Watch. If the evaluation method can’t find a nearby, paired Apple Watch running watchOS 6 or later, it returns the watchNotAvailable error.

During authentication, the system presents a dialog that resembles the dialog presented for biometric authentication. The user confirms authentication by double-clicking the watch’s side button.

To allow the user to authenticate either with an Apple Watch or with biometrics, use the LAPolicy.deviceOwnerAuthenticationWithBiometricsOrWatch policy instead. To allow the user to authenticate with either of these options or a password, use the LAPolicy.deviceOwnerAuthentication policy.

## See Also

### Policies

case deviceOwnerAuthenticationWithBiometrics

User authentication with biometry.

case deviceOwnerAuthenticationWithBiometricsOrWatch

User authentication with either biometry or Apple Watch.

Deprecated

case deviceOwnerAuthentication

User authentication with biometry, Apple Watch, or the device passcode.

case deviceOwnerAuthenticationWithWristDetection

User authentication with wrist detection on watchOS.

