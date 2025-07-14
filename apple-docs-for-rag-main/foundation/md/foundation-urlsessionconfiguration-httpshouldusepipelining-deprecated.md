

- Foundation
- URLSessionConfiguration
-  httpShouldUsePipelining Deprecated

Instance Property

# httpShouldUsePipelining

A Boolean value that determines whether the session should use HTTP pipelining.

iOS 7.0–18.4DeprecatediPadOS 7.0–18.4DeprecatedMac Catalyst 13.1–18.4DeprecatedmacOS 10.9–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–11.4Deprecated

``` source
var httpShouldUsePipelining: Bool { get set }
```

Deprecated

Only supported in the classic loader, please adopt HTTP/2 and HTTP/3 instead

## Discussion

This property determines whether tasks within sessions based on this configuration should use HTTP pipelining. You can also enable pipelining on a per-task basis by creating the task with an NSURLRequest object.

The default value is false.

## See Also

### Setting HTTP policy and proxy properties

var httpMaximumConnectionsPerHost: Int

The maximum number of simultaneous connections to make to a given host.

var proxyConfigurations: [ProxyConfiguration]

An array of proxy configuration objects containing information about the proxies to use within this session.

var connectionProxyDictionary: [AnyHashable : Any]?

A dictionary containing information about the proxy to use within this session.

