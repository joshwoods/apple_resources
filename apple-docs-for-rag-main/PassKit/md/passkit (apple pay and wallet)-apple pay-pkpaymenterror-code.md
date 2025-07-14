

- PassKit (Apple Pay and Wallet)
- Apple Pay
- PKPaymentError
-  code 

Instance Property

# code

The error code for this instance.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.5+macOS 10.10+visionOS 1.0+watchOS 2.0+Xcode 12.5+

``` source
var code: Code { get }
```

## Discussion

See PKPaymentError.Code for the list of error codes you can use for `errorCode`, which belong to the payment error domain (PKPaymentErrorDomain).

## See Also

### Describing the error

var errorCode: Int

The error code for this instance.

var userInfo: [String : Any]

Additional details about the error.

var errorUserInfo: [String : Any]

Additional details about the error.

