

- Local Authentication
- LAPolicy
-  LAPolicy.deviceOwnerAuthenticationWithBiometrics 

Case

# LAPolicy.deviceOwnerAuthenticationWithBiometrics

User authentication with biometry.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.12.2+visionOS 1.0+

``` source
case deviceOwnerAuthenticationWithBiometrics
```

## Discussion

You use the LAPolicy.deviceOwnerAuthenticationWithBiometrics policy when calling the evaluatePolicy(_:localizedReason:reply:) method to authenticate the user with biometrics.

Policy evaluation fails if Touch ID or Face ID is unavailable or not enrolled. Evaluation also fails after three failed Touch ID attempts. After two failed Face ID attempts, the system offers a fallback option, but stops trying to authenticate with Face ID. Both Touch ID and Face ID authentication are disabled system-wide after five consecutive unsuccessful attempts, even when the attempts span multiple evaluation calls. When this happens, the system requires the user to enter the device passcode to reenable biometry.

During authentication, the system presents the user with an authentication dialog for every attempt to authenticate with Touch ID, or after any failed Face ID attempt. The dialog contains a cancel button with a title that you can customize by setting the localizedCancelTitle property. If the user taps the cancel button, the policy evaluation fails with the userCancel error.

The authentication dialog also displays a fallback button after the first unsuccessful Touch ID attempt, or after the second unsuccessful Face ID attempt. You can customize the fallback button’s title by setting the localizedFallbackTitle property. If the user taps the fallback button, the policy evaluation fails with the userFallback error. In this case, your app should provide an alternate mechanism for authenticating the user, like asking for a PIN or a password.

To let the system handle the fallback option by asking for the device passcode (in iOS or watchOS) or the user’s password (in macOS), use the LAPolicy.deviceOwnerAuthentication policy instead.

## See Also

### Policies

case deviceOwnerAuthenticationWithWatch

User authentication with Apple Watch.

Deprecated

case deviceOwnerAuthenticationWithBiometricsOrWatch

User authentication with either biometry or Apple Watch.

Deprecated

case deviceOwnerAuthentication

User authentication with biometry, Apple Watch, or the device passcode.

case deviceOwnerAuthenticationWithWristDetection

User authentication with wrist detection on watchOS.

