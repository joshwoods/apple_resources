

- PassKit (Apple Pay and Wallet)
- Wallet
- PKAddSecureElementPassError
-  errorUserInfo 

Instance Property

# errorUserInfo

A dictionary that contains custom information that relates to the error.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.4+macOS 10.10+visionOS 1.0+watchOS 2.0+Xcode 11.4+

``` source
var errorUserInfo: [String : Any] { get }
```

## See Also

### Getting error information

let PKAddSecureElementPassErrorDomain: String

The error domain for errors that occur when adding a secure pass.

var code: Code

The code that provides context for the error.

var errorCode: Int

The code that provides context for the error.

var userInfo: [String : Any]

A dictionary that contains custom information that relates to the error.

