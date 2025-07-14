

- Network Extension
- NEProxySettings
-  excludeSimpleHostnames 

Instance Property

# excludeSimpleHostnames

A Boolean indicating if HTTP requests using single-label host names should be excluded from using the proxy settings.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var excludeSimpleHostnames: Bool { get set }
```

## See Also

### Accessing General Proxy Properties

var exceptionList: [String]?

An array of domain name patterns. If the destination host name of an HTTP connection matches one of these patterns then the proxy settings will not be used for the connection.

var matchDomains: [String]?

An array of domain strings.

