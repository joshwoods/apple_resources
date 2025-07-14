

- Core Foundation
-  CFStreamEventType 

Structure

# CFStreamEventType

Defines constants for stream-related events.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CFStreamEventType
```

## Overview

This enumeration defines constants for stream-related events.

## Topics

### Constants

static var openCompleted: CFStreamEventType

The open has completed successfully.

static var hasBytesAvailable: CFStreamEventType

The stream has bytes to be read.

static var canAcceptBytes: CFStreamEventType

The stream can accept bytes for writing.

static var errorOccurred: CFStreamEventType

An error has occurred on the stream.

static var endEncountered: CFStreamEventType

The end of the stream has been reached.

### Initializers

init(rawValue: CFOptionFlags)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

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

