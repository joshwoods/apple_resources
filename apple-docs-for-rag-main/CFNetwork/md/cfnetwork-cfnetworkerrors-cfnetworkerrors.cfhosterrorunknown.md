

- CFNetwork
- CFNetworkErrors
-  CFNetworkErrors.cfHostErrorUnknown 

Case

# CFNetworkErrors.cfHostErrorUnknown

An unknown error.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
case cfHostErrorUnknown
```

## Discussion

An unknown error (for example, a name server failure) occurred. For additional information, you can query the `kCFGetAddrInfoFailureKey` key to obtain the value returned by `getaddrinfo(_:_:_:_:)` and look up the value in `/usr/include/netdb.h`.

## See Also

### Constants

case cfHostErrorHostNotFound

The specified host wasn’t found.

case cfsocksErrorUnknownClientVersion

The SOCKS server rejected access because it doesn’t support connections with the requested SOCKS version.

case cfsocksErrorUnsupportedServerVersion

The SOCKS server doesn’t support the requested version.

case cfsocks4ErrorRequestFailed

The server rejected the request, or the request failed.

case cfsocks4ErrorIdentdFailed

The server couldn’t connect to the `identd` daemon on the client and rejected the request.

case cfsocks4ErrorIdConflict

The server rejected the request because the client program and the `identd` daemon reported different user IDs.

case cfsocks4ErrorUnknownStatusCode

The server returned an unknown status code.

case cfsocks5ErrorBadState

The stream isn’t in a state that allows the requested operation.

case cfsocks5ErrorBadResponseAddr

The address type returned isn’t supported.

case cfsocks5ErrorBadCredentials

The SOCKS server refused the client connection because of bad login credentials.

case cfsocks5ErrorUnsupportedNegotiationMethod

The requested method isn’t supported.

case cfsocks5ErrorNoAcceptableMethod

The client and server couldn’t find a mutually agreeable authentication method.

case cfftpErrorUnexpectedStatusCode

The server returned an unexpected status code.

case cfErrorHTTPAuthenticationTypeUnsupported

The client and server couldn’t agree on a supported authentication type.

case cfErrorHTTPBadCredentials

The server rejected the credentials provided for an authenticated connection.

