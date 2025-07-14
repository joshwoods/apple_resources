

- Core Foundation
-  kCFStreamSocketSecurityLevelSSLv3 Deprecated

Global Variable

# kCFStreamSocketSecurityLevelSSLv3

Specifies that SSL version 3 be set as the security protocol for a socket stream pair.

iOS 2.0–10.0DeprecatediPadOS 2.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.12DeprecatedtvOSDeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–3.0Deprecated

``` source
let kCFStreamSocketSecurityLevelSSLv3: CFString
```

## Discussion

If SSL version 3 is not available, specifies that SSL version 2 be set as the security protocol for a socket stream.

## See Also

### Constants

let kCFStreamSocketSecurityLevelNone: CFString

Specifies that no security level be set.

let kCFStreamSocketSecurityLevelSSLv2: CFString

Specifies that SSL version 2 be set as the security protocol for a socket stream.

Deprecated

let kCFStreamSocketSecurityLevelTLSv1: CFString

Specifies that TLS version 1 be set as the security protocol for a socket stream.

let kCFStreamSocketSecurityLevelNegotiatedSSL: CFString

Specifies that the highest level security protocol that can be negotiated be set as the security protocol for a socket stream.

