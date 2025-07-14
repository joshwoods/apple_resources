

- Core Foundation
-  CFStreamStatus 

Enumeration

# CFStreamStatus

Constants that describe the status of a stream.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CFStreamStatus
```

## Overview

The `CFStreamStatus` enumeration defines constants that describe the status of a stream. These values are returned by CFReadStreamGetStatus(_:) and CFWriteStreamGetStatus(_:).

## Topics

### Constants

case notOpen

The stream is not open for reading or writing.

case opening

The stream is being opened for reading or for writing.

case open

The stream is open.

case reading

The stream is being read from.

case writing

The stream is being written to.

case atEnd

There is no more data to read, or no more data can be written.

case closed

The stream is closed.

case error

An error occurred on the stream.

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

Stream Service Types

String constants that specify the service type of a stream.

