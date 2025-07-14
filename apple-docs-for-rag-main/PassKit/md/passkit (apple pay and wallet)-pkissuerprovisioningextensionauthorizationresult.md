

- PassKit (Apple Pay and Wallet)
-  PKIssuerProvisioningExtensionAuthorizationResult 

Enumeration

# PKIssuerProvisioningExtensionAuthorizationResult

A value that indicates the result of authorizing the addition of a payment card.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
enum PKIssuerProvisioningExtensionAuthorizationResult
```

## Topics

### Authorization results

case authorized

A result that indicates the user successfully authorized adding the payment pass.

case canceled

A result that indicates the user canceled authorization or wasn’t authorized to add the payment card.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Providing the result of authorization

var completionHandler: ((PKIssuerProvisioningExtensionAuthorizationResult) -> Void)?

A completion handler the system calls to find the result of authorizing the addition of the payment card.

**Required**

