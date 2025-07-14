

- Core Foundation
-  kCFStreamPropertySOCKSProxy 

Global Variable

# kCFStreamPropertySOCKSProxy

SOCKS proxy property key.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOSvisionOS 1.0+watchOS 2.0+

``` source
let kCFStreamPropertySOCKSProxy: CFString
```

## Discussion

To set a `CFStream` object to use a SOCKS proxy, call CFReadStreamSetProperty(_:_:_:) or CFWriteStreamSetProperty(_:_:_:) with the property name set to `kCFStreamPropertySOCKSProxy` and its value set to a `CFDictionary` object having at minimum a `kCFStreamPropertySOCKSProxyHost` key and a `kCFStreamPropertySOCKSProxyPort` key. For information on these keys, see CFStream SOCKS Proxy Key Constants. SystemConfiguration returns a CFDictionary for SOCKS proxies that is usable without modification.

## See Also

### Constants

static let appendToFile: CFStreamPropertyKey!

Value is a `CFBoolean` value that indicates whether to append the written data to a file, if it already exists, rather than to replace its contents.

static let dataWritten: CFStreamPropertyKey!

Value is a `CFData` object that contains all the bytes written to a writable memory stream. You cannot modify this value.

static let fileCurrentOffset: CFStreamPropertyKey!

Value is a `CFNumber` object containing the current file offset.

static let socketNativeHandle: CFStreamPropertyKey!

Value is a `CFData` object that contains the native handle for a socket stream—of type CFSocketNativeHandle—to which the socket stream is connected.

static let socketRemoteHostName: CFStreamPropertyKey!

Value is a `CFString` object containing the name of the host to which the socket stream is connected or `NULL` if unknown.

static let socketRemotePortNumber: CFStreamPropertyKey!

Value is a `CFNumber` object containing the remote port number to which the socket stream is connected or `NULL` if unknown.

let kCFStreamPropertyShouldCloseNativeSocket: CFString

Should Close Native Socket property key.

let kCFStreamPropertySocketSecurityLevel: CFString

Socket Security Level property key.

let kCFStreamPropertySSLPeerCertificates: CFString

SSL Peer Certificates property key for copy operations, which return a \`CFArray\` object containing \`SecCertificateRef\` objects.

Deprecated

let kCFStreamPropertySSLPeerTrust: CFString

SSL Peer Trust property key for copy operations, which return a \`SecTrustRef\` object containing the result of the SSL handshake.

let kCFStreamPropertySSLSettings: CFString

SSL Settings property key for set operations.

let kCFStreamPropertySSLContext: CFString

let kCFStreamPropertyProxyLocalBypass: CFString

Proxy Local Bypass property key.

let kCFStreamPropertySocketRemoteHost: CFString

The key’s value is a \`CFHostRef\` for the remote host if it is known. If not, its value is \`NULL\`.

let kCFStreamPropertySocketRemoteNetService: CFString

The key’s value is a \`CFNetServiceRef\` for the remote network service if it is known. If not, its value is \`NULL\`.

