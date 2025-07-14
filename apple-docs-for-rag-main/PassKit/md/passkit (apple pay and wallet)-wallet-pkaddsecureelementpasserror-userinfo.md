

- PassKit (Apple Pay and Wallet)
- Wallet
- PKAddSecureElementPassError
-  userInfo 

Instance Property

# userInfo

A dictionary that contains custom information that relates to the error.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.5+macOS 10.10+visionOS 1.0+watchOS 2.0+Xcode 12.5+

``` source
var userInfo: [String : Any] { get }
```

## See Also

### Getting error information

let PKAddSecureElementPassErrorDomain: String

The error domain for errors that occur when adding a secure pass.

var code: Code

The code that provides context for the error.

var errorCode: Int

The code that provides context for the error.

var errorUserInfo: [String : Any]

A dictionary that contains custom information that relates to the error.

