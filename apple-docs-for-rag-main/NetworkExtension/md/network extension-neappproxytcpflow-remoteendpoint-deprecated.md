

- Network Extension
- NEAppProxyTCPFlow
-  remoteEndpoint Deprecated

Instance Property

# remoteEndpoint

An NWEndpoint object containing information about the intended remote endpoint of the flow.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var remoteEndpoint: NWEndpoint { get }
```

## Discussion

If the flow’s corresponding socket was created using one of the high-level networking APIs such as URLSession or NSURLConnection, then the hostname property of the `remoteEndpoint` object contains the DNS name of the remote host. If the flow’s corresponding socket was created using the sockets API directly, then the hostname property of the `remoteEndpoint` object contains the IP address of the remote host.

