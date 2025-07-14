

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationResult
-  errors 

Instance Property

# errors

List of errors in the Apple Pay sheet.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var errors: [any Error]! { get set }
```

## Discussion

If the Apple Pay sheet contains errors, you provide a PKPaymentAuthorizationStatus.failure status to PKPaymentAuthorizationResult, and include the individual errors in this array. If there are no errors, you provide a PKPaymentAuthorizationStatus.success status and leave the error array empty. Errors are of the standard type, NSError. To create errors, you can either use the convenience methods found in PKPaymentRequest, or create an NSError using the domain, error codes, and user info from PKPaymentError.

Add the errors to the array in order of severity, with the most important error first.

## See Also

### Setting payment authorization status and errors

var status: PKPaymentAuthorizationStatus

Payment authorization general status.

enum PKPaymentAuthorizationStatus

General success and failure status for payment authorization.

