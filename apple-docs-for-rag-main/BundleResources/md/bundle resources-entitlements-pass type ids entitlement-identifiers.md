

- Bundle Resources
- Entitlements
-  Pass Type IDs Entitlement 

Property List Key

# Pass Type IDs Entitlement

A list of identifiers that specify pass types that your app can access in Wallet.

iOS 6.0+iPadOS 6.0+visionOS 1.0+watchOS 2.0+

## Details 

Key  
com.apple.developer.pass-type-identifiers

Type  

array of strings

## Discussion

The value for this key is an array of pass type identifiers.

To add this entitlement to your app, enable the Wallet capability in Xcode. If your provisioning profile is associated with multiple pass type identifiers, specify which of the identifiers your app can interact with. Use `$(TeamIdentifierPrefix)*` to access all of the passes for your team.

For more information, see Configure Wallet (iOS, watchOS).

Note

In iOS 17 and later, App Clips can use the Wallet capability. For more information on functionality that’s available to App Clips, see Choosing the right functionality for your App Clip.

## See Also

### Wallet

Merchant IDs Entitlement

A list of merchant IDs your app uses for Apple Pay support.

**Key:** com.apple.developer.in-app-payments

com.apple.developer.in-app-identity-presentment

com.apple.developer.in-app-identity-presentment.merchant-identifiers

ID Verifier - Display Only

ID Verifier - Data Transfer

