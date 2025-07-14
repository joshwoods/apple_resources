

- PassKit (Apple Pay and Wallet)
- PKIssuerProvisioningExtensionAuthorizationProviding
-  completionHandler 

Instance Property

# completionHandler

A completion handler the system calls to find the result of authorizing the addition of the payment card.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
var completionHandler: ((PKIssuerProvisioningExtensionAuthorizationResult) -> Void)? { get set }
```

**Required**

## Discussion

The completion handler takes the following parameter:

`result`  
A PKIssuerProvisioningExtensionAuthorizationResult case that indicates the result of authorizing the addition of the payment card.

## See Also

### Providing the result of authorization

enum PKIssuerProvisioningExtensionAuthorizationResult

A value that indicates the result of authorizing the addition of a payment card.

