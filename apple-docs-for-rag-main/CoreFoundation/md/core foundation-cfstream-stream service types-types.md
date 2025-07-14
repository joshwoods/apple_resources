

- Core Foundation
- CFStream
-  Stream Service Types 

# Stream Service Types

String constants that specify the service type of a stream.

## Topics

### Constants

let kCFStreamNetworkServiceTypeVoIP: CFString

Specifies that the stream is providing VoIP service.

Deprecated

let kCFStreamNetworkServiceTypeVideo: CFString

Specifies that the stream is providing interactive video data.

let kCFStreamNetworkServiceTypeBackground: CFString

Specifies that the stream is a background download.

let kCFStreamNetworkServiceTypeVoice: CFString

Specifies that the stream is providing interactive voice data.

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

CFStream SOCKS Proxy Key Constants

Constants for SOCKS Proxy `CFDictionary` keys.

