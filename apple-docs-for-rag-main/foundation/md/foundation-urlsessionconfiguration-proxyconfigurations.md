

- Foundation
- URLSessionConfiguration
-  proxyConfigurations 

Instance Property

# proxyConfigurations

An array of proxy configuration objects containing information about the proxies to use within this session.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var proxyConfigurations: [ProxyConfiguration] { get set }
```

## Discussion

This property controls which proxy tasks within sessions based on this configuration use when connecting to remote hosts.

The default value is the empty array, which means that tasks use the default system settings.

## See Also

### Setting HTTP policy and proxy properties

var httpMaximumConnectionsPerHost: Int

The maximum number of simultaneous connections to make to a given host.

var httpShouldUsePipelining: Bool

A Boolean value that determines whether the session should use HTTP pipelining.

Deprecated

var connectionProxyDictionary: [AnyHashable : Any]?

A dictionary containing information about the proxy to use within this session.

