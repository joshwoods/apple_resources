

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationResult
-  status 

Instance Property

# status

Payment authorization general status.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var status: PKPaymentAuthorizationStatus { get set }
```

## Discussion

See PKPaymentAuthorizationStatus for the list of status values.

## See Also

### Setting payment authorization status and errors

var errors: [any Error]!

List of errors in the Apple Pay sheet.

enum PKPaymentAuthorizationStatus

General success and failure status for payment authorization.

