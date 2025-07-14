

- PassKit (Apple Pay and Wallet)
- PKPaymentRequestUpdate
-  status 

Instance Property

# status

The status of the payment request that indicates whether authorization succeeds or fails.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var status: PKPaymentAuthorizationStatus { get set }
```

## Discussion

See PKPaymentAuthorizationStatus for valid values.

## See Also

### Updating authorization status

enum PKPaymentAuthorizationStatus

General success and failure status for payment authorization.

