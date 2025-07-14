

- PassKit (Apple Pay and Wallet)
- Apple Pay
- PKPaymentError
-  userInfo 

Instance Property

# userInfo

Additional details about the error.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.5+macOS 10.10+visionOS 1.0+watchOS 2.0+Xcode 12.5+

``` source
var userInfo: [String : Any] { get }
```

## Discussion

Use PKPaymentErrorKey values in the `errorUserInfo` property to provide more details for an error, for example, to indicate the part of the address that’s incorrect.

## See Also

### Describing the error

var code: Code

The error code for this instance.

var errorCode: Int

The error code for this instance.

var errorUserInfo: [String : Any]

Additional details about the error.

