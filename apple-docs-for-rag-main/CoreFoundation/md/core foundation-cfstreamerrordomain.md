

- Core Foundation
-  CFStreamErrorDomain 

Enumeration

# CFStreamErrorDomain

Defines constants for values returned in the domain field of the `CFStreamError` structure.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CFStreamErrorDomain
```

## Overview

These constants indicate how the error code in the `error` field in the CFStreamError structure should be interpreted.

## Topics

### Constants

case custom

The error code is a custom error code.

Deprecated

case POSIX

The error code is an error code defined in `errno.h`.

case macOSStatus

The error is an OSStatus value defined in `MacErrors.h`.

### Initializers

init?(rawValue: CFIndex)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum CFStreamStatus

Constants that describe the status of a stream.

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

Stream Service Types

String constants that specify the service type of a stream.

