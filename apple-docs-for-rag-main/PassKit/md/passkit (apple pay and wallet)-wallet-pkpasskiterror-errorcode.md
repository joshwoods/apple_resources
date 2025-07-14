

- PassKit (Apple Pay and Wallet)
- Wallet
- PKPassKitError
-  errorCode 

Instance Property

# errorCode

The code that provides context for the error.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+visionOS 1.0+watchOS 2.0+Xcode 8.0+

``` source
var errorCode: Int { get }
```

## Discussion

Errors are domain-specific. See PKPassKitError.Code for more information.

## See Also

### Error information

var code: Code

The code that provides context for the error.

var userInfo: [String : Any]

A dictionary that contains custom information that relates to the error.

var errorUserInfo: [String : Any]

A dictionary that contains custom information that relates to the error.

