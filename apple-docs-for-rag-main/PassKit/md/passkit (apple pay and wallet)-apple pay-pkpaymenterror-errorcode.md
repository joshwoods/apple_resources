

- PassKit (Apple Pay and Wallet)
- Apple Pay
- PKPaymentError
-  errorCode 

Instance Property

# errorCode

The error code for this instance.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+visionOS 1.0+watchOS 2.0+Xcode 9.0+

``` source
var errorCode: Int { get }
```

## Discussion

See PKPaymentError.Code for the list of error codes you can use for `errorCode`, which belong to the payment error domain (PKPaymentErrorDomain).

## See Also

### Describing the error

var code: Code

The error code for this instance.

var userInfo: [String : Any]

Additional details about the error.

var errorUserInfo: [String : Any]

Additional details about the error.

