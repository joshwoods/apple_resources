

- CFNetwork
-  kCFNetworkProxiesHTTPSProxy 

Global Variable

# kCFNetworkProxiesHTTPSProxy

Value is a `CFString` object containing the HTTPS proxy host name or IP number.

macOS 10.6+

``` source
let kCFNetworkProxiesHTTPSProxy: CFString
```

## See Also

### Constants

let kCFNetworkProxiesExceptionsList: CFString

Value is a `CFArray` of `CFString` objects indicating host name patterns that should bypass the proxy.

let kCFNetworkProxiesExcludeSimpleHostnames: CFString

Value is a `CFNumber` object indicating whether simple host names are excluded. Simple host names are excluded if the key is present and the associated value is nonzero.

let kCFNetworkProxiesFTPEnable: CFString

Value is a `CFNumber` object indicating whether an FTP proxy is enabled. The proxy is enabled if the key is present and the associated value is nonzero.

let kCFNetworkProxiesFTPPassive: CFString

Value is a `CFNumber` object indicating whether an FTP proxy’s passive mode is enabled. The passive mode is enabled if the key is present and the associated value is nonzero.

let kCFNetworkProxiesFTPPort: CFString

Value is a `CFNumber` object indicating the port number of an FTP proxy.

let kCFNetworkProxiesFTPProxy: CFString

Value is a `CFString` object indicating the host name or IP number of an FTP proxy.

let kCFNetworkProxiesGopherEnable: CFString

Value is a `CFNumber` object indicating whether a gopher proxy is enabled. The proxy is enabled if the key is present and the associated value is nonzero.

let kCFNetworkProxiesGopherPort: CFString

Value is a `CFNumber` indicating the port number of a gopher proxy.

let kCFNetworkProxiesGopherProxy: CFString

Value is a `CFString` object indicating the host name or IP number of a gopher proxy.

let kCFNetworkProxiesHTTPEnable: CFString

Value is a `CFNumber` object indicating whether an HTTP proxy is enabled. The proxy is enabled if the key is present and the associated value is nonzero.

let kCFNetworkProxiesHTTPPort: CFString

Value is a `CFNumber` object containing the port number associated with the HTTP proxy.

let kCFNetworkProxiesHTTPProxy: CFString

Value is a `CFString` object containing the HTTP proxy host name or IP number.

let kCFNetworkProxiesHTTPSEnable: CFString

Value is a `CFNumber` object indicating whether an HTTPS proxy is enabled. The proxy is enabled if the key is present and the associated value is nonzero.

let kCFNetworkProxiesHTTPSPort: CFString

Value is a `CFNumber` object containing the port number associated with the HTTPS proxy.

let kCFNetworkProxiesRTSPEnable: CFString

Value is a `CFNumber` object indicating whether an RTSP proxy is enabled. The proxy is enabled if the key is present and the associated value is nonzero.

