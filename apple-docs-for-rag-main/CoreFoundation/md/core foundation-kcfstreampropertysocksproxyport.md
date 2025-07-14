

- Core Foundation
-  kCFStreamPropertySOCKSProxyPort 

Global Variable

# kCFStreamPropertySOCKSProxyPort

Constant for the SOCKS proxy host port key.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOSvisionOS 1.0+watchOS 2.0+

``` source
let kCFStreamPropertySOCKSProxyPort: CFString
```

## Discussion

This key contains a `CFNumberRef` object of type `kCFNumberSInt32Type` whose value represents the port on which the proxy listens.

## See Also

### Constants

let kCFStreamPropertySOCKSProxyHost: CFString

Constant for the SOCKS proxy host key.

let kCFStreamPropertySOCKSVersion: CFString

Constant for the SOCKS version key.

let kCFStreamSocketSOCKSVersion4: CFString

Constant used in the `kCFStreamSockerSOCKSVersion` key to specify SOCKS4 as the SOCKS version for the stream.

let kCFStreamSocketSOCKSVersion5: CFString

Constant used in the `kCFStreamSOCKSVersion` key to specify SOCKS5 as the SOCKS version for the stream.

let kCFStreamPropertySOCKSUser: CFString

Constant for the key required to set a user name.

let kCFStreamPropertySOCKSPassword: CFString

Constant for the key required to set a user’s password.

