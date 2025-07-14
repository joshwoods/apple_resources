

- Foundation
-  NSURLAuthenticationMethodHTMLForm 

Global Variable

# NSURLAuthenticationMethodHTMLForm

Use HTML form authentication for this protection space.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let NSURLAuthenticationMethodHTMLForm: String
```

## Discussion

The URL loading system never issues authentication challenges based on this authentication method. However, if your app authenticates by submitting a web form (or in some other protocol-neutral way), you can specify this protection space when you persist or look up credentials using the URLCredentialStorage class.

## See Also

### Task-specific authentication challenges

let NSURLAuthenticationMethodDefault: String

Use the default authentication method for a protocol.

let NSURLAuthenticationMethodHTTPBasic: String

Use HTTP basic authentication for this protection space.

let NSURLAuthenticationMethodHTTPDigest: String

Use HTTP digest authentication for this protection space.

