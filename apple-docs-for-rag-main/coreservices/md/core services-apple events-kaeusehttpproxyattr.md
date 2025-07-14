

- Core Services
- Apple Events
-  kAEUseHTTPProxyAttr 

# kAEUseHTTPProxyAttr

Web Services Proxy support—these constants should be added as attributes of the event that is being sent (not as part of the direct object).

## Topics

### Constants

var kAEUseHTTPProxyAttr: Int

A value of type `typeBoolean`. Specifies whether to manually specify the proxy host and port. Defaults to `true`.

var kAEHTTPProxyPortAttr: Int

A value of type `typeSInt32`.

var kAEHTTPProxyHostAttr: Int

A value of type `typeChar` or `typeUTF8Text`.

