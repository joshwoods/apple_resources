

- PassKit (Apple Pay and Wallet)
- Apple Pay
- PKDisbursementError
-  errorCode 

Instance Property

# errorCode

An integer value that represents the error code.

iOS 8.0+iPadOS 8.0+Mac Catalyst 17.0+macOS 10.10+visionOS 1.0+Xcode 6.0.1+

``` source
var errorCode: Int { get }
```

## See Also

### Error details

enum PKDisbursementError.Code

Values that describe errors that can occur while processing the disbursement.

var code: Code

The code that describes the error.

var errorUserInfo: [String : Any]

A dictionary that contains additional details about the error.

var hashValue: Int

The hash value.

var userInfo: [String : Any]

A dictionary that contains additional details about the error.

