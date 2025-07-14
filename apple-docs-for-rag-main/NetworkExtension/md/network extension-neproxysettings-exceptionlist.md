

- Network Extension
- NEProxySettings
-  exceptionList 

Instance Property

# exceptionList

An array of domain name patterns. If the destination host name of an HTTP connection matches one of these patterns then the proxy settings will not be used for the connection.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var exceptionList: [String]? { get set }
```

## Discussion

The pattern strings may contain ‘\*’ characters as wildcards.

## See Also

### Accessing General Proxy Properties

var excludeSimpleHostnames: Bool

A Boolean indicating if HTTP requests using single-label host names should be excluded from using the proxy settings.

var matchDomains: [String]?

An array of domain strings.

