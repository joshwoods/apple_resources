

- Core Foundation
- CFStream
-  Stream Properties 

API Collection

# Stream Properties

Stream property names that can be set or copied.

## Overview

Use CFReadStreamCopyProperty(_:_:) or CFWriteStreamCopyProperty(_:_:) to read the property values. Use CFReadStreamSetProperty(_:_:_:) or CFWriteStreamSetProperty(_:_:_:) to set the property values.

## Topics

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

let kCFStreamPropertySOCKSProxy: CFString

SOCKS proxy property key.

let kCFStreamPropertyProxyLocalBypass: CFString

Proxy Local Bypass property key.

let kCFStreamPropertySocketRemoteHost: CFString

The key’s value is a \`CFHostRef\` for the remote host if it is known. If not, its value is \`NULL\`.

let kCFStreamPropertySocketRemoteNetService: CFString

The key’s value is a \`CFNetServiceRef\` for the remote network service if it is known. If not, its value is \`NULL\`.

let kCFStreamNetworkServiceType: CFString

The type of service for the stream. Providing the service type allows the system to properly handle certain attributes of the stream, including routing and suspension behavior. Most streams do not need to set this property. See \[Stream Service Types\](doc://com.apple.documentation/documentation/CoreFoundation/stream-service-types) for a list of possible values.

let kCFStreamPropertyConnectionIsCellular: CFString

A boolean value indicating whether the stream is connected over a cellular (WWAN) interface. This is a read-only property, and is \`false\` until the connection has been established.

let kCFStreamPropertyNoCellular: CFString

A Boolean value indicating that the connection should not be established over a cellular (WWAN) connection. This value can only be set \*before\* you open the stream.

## See Also

### Constants

enum CFStreamStatus

Constants that describe the status of a stream.

enum CFStreamErrorDomain

Defines constants for values returned in the domain field of the `CFStreamError` structure.

CFStream Error Domain Constants (CFHost)

Defines constants for values returned in the domain field of the `CFStreamError` structure.

Error Subdomains

Subdomains used to determine how to interpret an error in the `kCFStreamErrorDomainSOCKS` domain.

Secure Sockets (SOCKS) Errors

Error codes returned by the \`kCFStreamErrorDomainSOCKS\` error domain.

struct CFStreamEventType

Defines constants for stream-related events.

CFStream Property SSL Settings Constants

Constants for use in a `CFDictionary` object that is the value of the `kCFStreamPropertySSLSettings` stream property key.

CFStream Socket Security Level Constants

Constants for setting the security level of a socket stream.

CFStream SOCKS Proxy Key Constants

Constants for SOCKS Proxy `CFDictionary` keys.

Stream Service Types

String constants that specify the service type of a stream.

