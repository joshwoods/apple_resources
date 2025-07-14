

- Core Foundation
- CFStream
-  CFStream Property SSL Settings Constants 

# CFStream Property SSL Settings Constants

Constants for use in a `CFDictionary` object that is the value of the `kCFStreamPropertySSLSettings` stream property key.

## Overview

This enumeration defines the constants for keys in a `CFDictionary` object that is the value of the kCFStreamPropertySSLSettings key.

## Topics

### Constants

let kCFStreamSSLLevel: CFString

Security property key whose value specifies the stream’s security level.

let kCFStreamSSLAllowsExpiredCertificates: CFString

Security property key whose value indicates whether expired certificates are allowed.

Deprecated

let kCFStreamSSLAllowsExpiredRoots: CFString

Security property whose value indicates whether expired root certificates are allowed.

Deprecated

let kCFStreamSSLAllowsAnyRoot: CFString

Security property key whose value indicates whether root certificates should be allowed.

Deprecated

let kCFStreamSSLValidatesCertificateChain: CFString

Security property key whose value indicates whether the certificate chain should be validated.

let kCFStreamSSLPeerName: CFString

Security property key whose value overrides the name used for certificate verification.

let kCFStreamSSLCertificates: CFString

Security property key whose value is a CFArray of SecCertificateRefs except for the first element in the array, which is a SecIdentityRef.

let kCFStreamSSLIsServer: CFString

Security property key whose value indicates whether the connection is to act as a server in the SSL process.

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

Stream Properties

Stream property names that can be set or copied.

CFStream Socket Security Level Constants

Constants for setting the security level of a socket stream.

CFStream SOCKS Proxy Key Constants

Constants for SOCKS Proxy `CFDictionary` keys.

Stream Service Types

String constants that specify the service type of a stream.

