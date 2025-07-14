

- PassKit (Apple Pay and Wallet)
- PKDisbursementRequest
-  applicationData 

Instance Property

# applicationData

Optional merchant-supplied information about the disbursement request.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 15.0+visionOS 1.0+

``` source
var applicationData: Data? { get set }
```

## Discussion

The system hashes the data and includes it in the resulting PKPaymentToken.

