

- Foundation
- URLRequest
-  httpShouldUsePipelining Deprecated

Instance Property

# httpShouldUsePipelining

A Boolean value indicating whether the request should transmit before the previous response is received.

iOS 8.0–18.4DeprecatediPadOS 8.0–18.4DeprecatedMac Catalyst 8.0–18.4DeprecatedmacOS 10.10–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–11.4Deprecated

``` source
var httpShouldUsePipelining: Bool { get set }
```

Deprecated

Only supported in the classic loading mode, please adopt HTTP/2 and HTTP/3 instead

## See Also

### Controlling request behavior

var timeoutInterval: TimeInterval

The timeout interval of the request.

var httpShouldHandleCookies: Bool

A Boolean value indicating whether cookies will be sent with and set for this request.

var allowsCellularAccess: Bool

A Boolean value indicating whether the request is allowed to use the built-in cellular radios to satisfy the request.

var allowsPersistentDNS: Bool

var assumesHTTP3Capable: Bool

var cookiePartitionIdentifier: String?

var requiresDNSSECValidation: Bool

