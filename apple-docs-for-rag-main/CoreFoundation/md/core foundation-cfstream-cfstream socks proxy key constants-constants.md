

- Core Foundation
- CFStream
-  CFStream SOCKS Proxy Key Constants 

API Collection

# CFStream SOCKS Proxy Key Constants

Constants for SOCKS Proxy `CFDictionary` keys.

## Overview

When setting the stream’s SOCKS Proxy property, the property’s value is a `CFDictionary` object containing at minimum the kCFStreamPropertySOCKSProxyHost and kCFStreamPropertySOCKSProxyPort keys. The dictionary may also contain the other keys described in this section.

## Topics

### Constants

let kCFStreamPropertySOCKSProxyHost: CFString

Constant for the SOCKS proxy host key.

let kCFStreamPropertySOCKSProxyPort: CFString

Constant for the SOCKS proxy host port key.

let kCFStreamPropertySOCKSVersion: CFString

Constant for the SOCKS version key.

let kCFStreamSocketSOCKSVersion4: CFString

Constant used in the `kCFStreamSockerSOCKSVersion` key to specify SOCKS4 as the SOCKS version for the stream.

let kCFStreamSocketSOCKSVersion5: CFString

Constant used in the `kCFStreamSOCKSVersion` key to specify SOCKS5 as the SOCKS version for the stream.

let kCFStreamPropertySOCKSUser: CFString

Constant for the key required to set a user name.

let kCFStreamPropertySOCKSPassword: CFString

Constant for the key required to set a user’s password.

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

CFStream Property SSL Settings Constants

Constants for use in a `CFDictionary` object that is the value of the `kCFStreamPropertySSLSettings` stream property key.

CFStream Socket Security Level Constants

Constants for setting the security level of a socket stream.

Stream Service Types

String constants that specify the service type of a stream.

