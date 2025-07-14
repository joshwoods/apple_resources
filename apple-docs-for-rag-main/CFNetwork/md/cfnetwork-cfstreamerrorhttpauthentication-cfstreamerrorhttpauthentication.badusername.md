

- CFNetwork
- CFStreamErrorHTTPAuthentication
-  CFStreamErrorHTTPAuthentication.badUserName 

Case

# CFStreamErrorHTTPAuthentication.badUserName

User name is in a format that is not suitable for the request. Currently, user names are decoded using `kCFStringEncodingISOLatin1`.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
case badUserName
```

## See Also

### Constants

case typeUnsupported

Specified authentication type is not supported.

case badPassword

Password is in a format that is not suitable for the request. Currently, passwords are decoded using `kCFStringEncodingISOLatin1`.

