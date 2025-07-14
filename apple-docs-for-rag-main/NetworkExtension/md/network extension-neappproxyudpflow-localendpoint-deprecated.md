

- Network Extension
- NEAppProxyUDPFlow
-  localEndpoint Deprecated

Instance Property

# localEndpoint

An NWEndpoint object containing information about the local endpoint of the flow.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var localEndpoint: NWEndpoint? { get }
```

## Discussion

This property may be nil if the corresponding UDP socket was not bound to a port by the application and the App Proxy Provider did not set a local endpoint in open(withLocalEndpoint:completionHandler:).

