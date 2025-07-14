

- PassKit (Apple Pay and Wallet)
- Apple Pay
- PKDisbursementError
-  errorUserInfo 

Instance Property

# errorUserInfo

A dictionary that contains additional details about the error.

iOS 8.0+iPadOS 8.0+Mac Catalyst 17.0+macOS 10.10+visionOS 1.0+Xcode 6.0.1+

``` source
var errorUserInfo: [String : Any] { get }
```

## See Also

### Error details

enum PKDisbursementError.Code

Values that describe errors that can occur while processing the disbursement.

var code: Code

The code that describes the error.

var errorCode: Int

An integer value that represents the error code.

var hashValue: Int

The hash value.

var userInfo: [String : Any]

A dictionary that contains additional details about the error.

