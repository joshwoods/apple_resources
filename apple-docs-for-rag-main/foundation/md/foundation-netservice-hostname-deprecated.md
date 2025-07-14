

- Foundation
- NetService
-  hostName Deprecated

Instance Property

# hostName

A string containing the DNS hostname for this service.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.2–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4Deprecated

``` source
var hostName: String? { get }
```

Deprecated

Use nw_connection_t or nw_listener_t in Network framework instead

## Discussion

This value is `nil` until the service has been resolved (when `addresses` is non-`nil`).

