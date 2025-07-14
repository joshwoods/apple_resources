

- Bundle Resources
- Entitlements
-  Merchant IDs Entitlement 

Property List Key

# Merchant IDs Entitlement

A list of merchant IDs your app uses for Apple Pay support.

iOS 6.0+iPadOS 6.0+visionOS 1.0+watchOS 2.0+

## Details 

Key  
com.apple.developer.in-app-payments

Type  

array of strings

## Discussion

The value for this key is an array of strings containing the merchant IDs—typically in reverse domain name notation, starting with the string ‘`merchant`’.

To add this entitlement, enable the Apple Pay capability in Xcode and select the merchant IDs you want to use in your app. Alternatively, see Setting up Apple Pay for how to create merchant IDs in your developer account.

## See Also

### Wallet

Pass Type IDs Entitlement

A list of identifiers that specify pass types that your app can access in Wallet.

**Key:** com.apple.developer.pass-type-identifiers

com.apple.developer.in-app-identity-presentment

com.apple.developer.in-app-identity-presentment.merchant-identifiers

ID Verifier - Display Only

ID Verifier - Data Transfer

