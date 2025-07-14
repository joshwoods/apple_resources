

- PassKit (Apple Pay and Wallet)
- PKIssuerProvisioningExtensionStatus
-  requiresAuthentication 

Instance Property

# requiresAuthentication

A Boolean value that indicates whether adding a card requires an authorization-user-interface extension provided by your app.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOSvisionOS 1.0+

``` source
var requiresAuthentication: Bool { get set }
```

## Discussion

If you return `true` your app must provide a PKIssuerProvisioningExtensionAuthorizationProviding UI extension.

