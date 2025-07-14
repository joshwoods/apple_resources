

- CFNetwork
-  kSOCKS5NoAcceptableMethod 

Global Variable

# kSOCKS5NoAcceptableMethod

The client and server couldn’t find a mutually agreeable authentication method.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
var kSOCKS5NoAcceptableMethod: Int { get }
```

## Discussion

This error code is only valid for errors in the `kCFStreamErrorSOCKS5SubDomainMethod` subdomain.

## See Also

### Constants

var kCFStreamErrorSOCKS4IdConflict: Int

Request rejected by the server because the client program and the `identd` daemon reported different user IDs.

var kCFStreamErrorSOCKS4IdentdFailed: Int

Request rejected by the server because it couldn’t connect to the `identd` daemon on the client.

var kCFStreamErrorSOCKS4RequestFailed: Int

Request rejected by the server or request failed.

var kCFStreamErrorSOCKS4SubDomainResponse: Int

The SOCKS4 status code returned by the server.

var kCFStreamErrorSOCKS5SubDomainMethod: Int

The server’s desired negotiation method.

var kCFStreamErrorSOCKS5SubDomainResponse: Int

The response code that the server returned in reply to the connection request.

var kCFStreamErrorSOCKS5SubDomainUserPass: Int

The status code that the server returned during authentication.

var kCFStreamErrorSOCKSSubDomainNone: Int

A general SOCKS error.

var kCFStreamErrorSOCKSSubDomainVersionCode: Int

The version of SOCKS that the server wants to use.

var kCFStreamErrorSOCKS5BadResponseAddr: Int

The address returned is not of a known type. This error code is only valid for errors in the `kCFStreamErrorSOCKSSubDomainNone` subdomain.

var kCFStreamErrorSOCKS5BadState: Int

The stream is not in a state that allows the requested operation. This error code is only valid for errors in the `kCFStreamErrorSOCKSSubDomainNone` subdomain..

var kCFStreamErrorSOCKSUnknownClientVersion: Int

The SOCKS server rejected access because it does not support connections with the requested SOCKS version. SOCKS client version. You can query the `kCFSOCKSVersionKey` key to find out what version the server requested. This error code is only valid for errors in the `kCFStreamErrorSOCKSSubDomainNone` subdomain.

