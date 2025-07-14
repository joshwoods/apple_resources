

- PassKit (Apple Pay and Wallet)
- Apple Pay
- PKPaymentError
-  errorUserInfo 

Instance Property

# errorUserInfo

Additional details about the error.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+visionOS 1.0+watchOS 2.0+Xcode 9.0+

``` source
var errorUserInfo: [String : Any] { get }
```

## Discussion

Use PKPaymentErrorKey values in the `errorUserInfo` property to provide more details for an error, for example, to indicate the part of the address that’s incorrect.

## See Also

### Describing the error

var code: Code

The error code for this instance.

var errorCode: Int

The error code for this instance.

var userInfo: [String : Any]

Additional details about the error.

