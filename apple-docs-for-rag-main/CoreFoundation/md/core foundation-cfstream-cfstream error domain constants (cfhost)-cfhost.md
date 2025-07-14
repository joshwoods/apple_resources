

- Core Foundation
- CFStream
-  CFStream Error Domain Constants (CFHost) 

API Collection

# CFStream Error Domain Constants (CFHost)

Defines constants for values returned in the domain field of the `CFStreamError` structure.

## Overview

These constants indicate how the error code in the `error` field in the CFStreamError structure should be interpreted.

## Topics

### Constants

let kCFStreamErrorDomainNetDB: Int32

The error code is an error code defined in \`netdb.h\`.

let kCFStreamErrorDomainNetServices: Int32

The error code is a \`CFNetService\` error code. For details, see the \[\`CFNetServicesError\`\](doc://com.apple.cfnetwork/documentation/CFNetwork/CFNetServicesError) enumeration.

let kCFStreamErrorDomainMach: Int32

The error code is a Mach error code defined in \`mach/error.h\`.

let kCFStreamErrorDomainFTP: Int32

The error code is an FTP error code.

let kCFStreamErrorDomainHTTP: Int32

The error code is an HTTP error code.

let kCFStreamErrorDomainSystemConfiguration: Int32

The error code is a system configuration error code as defined in \`System/ConfigurationSystemConfiguration.h\`.

let kCFStreamErrorDomainWinSock: CFIndex

When running CFNetwork code on Windows, this domain returns error codes associated with the underlying TCP/IP stack. You should also note that non-networking errors such as \`ENOMEM\` are delivered through the POSIX domain. See the header \`winsock2.h\` for relevant error codes.

let kCFStreamErrorDomainSOCKS: Int32

The error code is a SOCKS proxy error.

let kCFStreamErrorDomainSSL: Int32

The error code is an SSL error code as defined in `Security/SecureTransport.h`.

## See Also

### Constants

enum CFStreamStatus

Constants that describe the status of a stream.

enum CFStreamErrorDomain

Defines constants for values returned in the domain field of the `CFStreamError` structure.

Error Subdomains

Subdomains used to determine how to interpret an error in the `kCFStreamErrorDomainSOCKS` domain.

Secure Sockets (SOCKS) Errors

Error codes returned by the \`kCFStreamErrorDomainSOCKS\` error domain.

struct CFStreamEventType

Defines constants for stream-related events.

Stream Properties

Stream property names that can be set or copied.

CFStream Property SSL Settings Constants

Constants for use in a `CFDictionary` object that is the value of the `kCFStreamPropertySSLSettings` stream property key.

CFStream Socket Security Level Constants

Constants for setting the security level of a socket stream.

CFStream SOCKS Proxy Key Constants

Constants for SOCKS Proxy `CFDictionary` keys.

Stream Service Types

String constants that specify the service type of a stream.

