

- Core Foundation
-  kCFStreamPropertyShouldCloseNativeSocket 

Global Variable

# kCFStreamPropertyShouldCloseNativeSocket

Should Close Native Socket property key.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOSvisionOS 1.0+watchOS 2.0+

``` source
let kCFStreamPropertyShouldCloseNativeSocket: CFString
```

## Discussion

If set to `kCFBooleanTrue`, the stream will close and release the underlying native socket when the stream is released. If set to `kCFBooleanFalse`, the stream will not close and release the underlying native socket when the stream is released. If a stream is created with a native socket, the default value of this property is `kCFBooleanFalse`. This property is only available for socket streams. It can be set by calling CFReadStreamSetProperty(_:_:_:) and CFWriteStreamSetProperty(_:_:_:), and it can be copied by CFReadStreamCopyProperty(_:_:) and CFWriteStreamCopyProperty(_:_:).

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

let kCFStreamPropertySOCKSProxy: CFString

SOCKS proxy property key.

let kCFStreamPropertyProxyLocalBypass: CFString

Proxy Local Bypass property key.

let kCFStreamPropertySocketRemoteHost: CFString

The key’s value is a \`CFHostRef\` for the remote host if it is known. If not, its value is \`NULL\`.

let kCFStreamPropertySocketRemoteNetService: CFString

The key’s value is a \`CFNetServiceRef\` for the remote network service if it is known. If not, its value is \`NULL\`.

