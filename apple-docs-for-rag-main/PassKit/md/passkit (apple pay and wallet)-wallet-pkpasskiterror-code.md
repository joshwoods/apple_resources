

- PassKit (Apple Pay and Wallet)
- Wallet
- PKPassKitError
-  code 

Instance Property

# code

The code that provides context for the error.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.5+macOS 10.10+visionOS 1.0+watchOS 2.0+Xcode 12.5+

``` source
var code: Code { get }
```

## Discussion

Errors are domain-specific. See PKPassKitError.Code for more information.

## See Also

### Error information

var errorCode: Int

The code that provides context for the error.

var userInfo: [String : Any]

A dictionary that contains custom information that relates to the error.

var errorUserInfo: [String : Any]

A dictionary that contains custom information that relates to the error.

