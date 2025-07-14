

- Local Authentication
- LAPolicy
-  LAPolicy.deviceOwnerAuthentication 

Case

# LAPolicy.deviceOwnerAuthentication

User authentication with biometry, Apple Watch, or the device passcode.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 3.0+

``` source
case deviceOwnerAuthentication
```

## Discussion

You use the LAPolicy.deviceOwnerAuthentication policy when calling the evaluatePolicy(_:localizedReason:reply:) method to authenticate a user in iOS with either biometrics or a passcode, in watchOS with a passcode, or in macOS with Touch ID, Apple Watch, or the user’s password.

If biometry is available, enrolled, and not disabled, the system uses that first. In macOS, the system simultaneously looks for a nearby, paired Apple Watch running watchOS 6 or later, and tries to use that in parallel. When these options aren’t available, the system prompts the user for the device passcode or user’s password.

In iOS, policy evaluation fails with the error passcodeNotSet if the device passcode isn’t enabled. The system disables passcode authentication after 6 unsuccessful attempts, with progressively increasing delays between attempts.

The authentication dialog contains a cancel button with a default title that you can customize using the localizedCancelTitle property, as well as a fallback button that you can customize using localizedFallbackTitle property. When the user taps the fallback button, the system reverts to asking for the device passcode or user’s password. When the user taps the cancel button, the evaluation fails with the userCancel error.

## See Also

### Policies

case deviceOwnerAuthenticationWithBiometrics

User authentication with biometry.

case deviceOwnerAuthenticationWithWatch

User authentication with Apple Watch.

Deprecated

case deviceOwnerAuthenticationWithBiometricsOrWatch

User authentication with either biometry or Apple Watch.

Deprecated

case deviceOwnerAuthenticationWithWristDetection

User authentication with wrist detection on watchOS.

