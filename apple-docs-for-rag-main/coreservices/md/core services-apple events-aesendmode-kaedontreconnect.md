

- Core Services
- Apple Events
- AESendMode
-  kAEDontReconnect 

Global Variable

# kAEDontReconnect

Mac Catalyst 13.0+macOS 10.0+

``` source
var kAEDontReconnect: Int { get }
```

## Discussion

Deprecated and unsupported in macOS. The reconnection preference—the Apple Event Manager must not automatically try to reconnect if it receives a `sessClosedErr` result code from the PPC Toolbox. If you don’t set this flag, the Apple Event Manager automatically attempts to reconnect and reestablish the session.

