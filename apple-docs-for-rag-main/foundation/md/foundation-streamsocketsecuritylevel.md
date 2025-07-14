

- Foundation
-  StreamSocketSecurityLevel 

Structure

# StreamSocketSecurityLevel

`NSStream` defines these string constants for specifying the secure-socket layer (SSL) security level.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct StreamSocketSecurityLevel
```

## Discussion

You access and set these values using the `NSStreamSocketSecurityLevelKey` property key.

## Topics

### Type Properties

static let negotiatedSSL: StreamSocketSecurityLevel

Specifies that the highest level security protocol that can be negotiated be set as the security protocol for a socket stream.

static let none: StreamSocketSecurityLevel

Specifies that no security level be set for a socket stream.

static let ssLv2: StreamSocketSecurityLevel

Specifies that SSL version 2 be set as the security protocol for a socket stream.

static let ssLv3: StreamSocketSecurityLevel

Specifies that SSL version 3 be set as the security protocol for a socket stream.

static let tlSv1: StreamSocketSecurityLevel

Specifies that TLS version 1 be set as the security protocol for a socket stream.

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum Status

The type declared for the constants listed in doc:stream/stream_status_constants.

Stream Status Constants

These constants indicate the current status of a stream. They are returned by streamStatus.

struct Event

Describes the constants that may be sent to the delegate as a bit field in the second parameter of stream(_:handle:) to specify the kind of stream event.

struct StreamNetworkServiceTypeValue

`NSStream` defines these string constants for specifying the service type of a stream.

struct StreamSOCKSProxyConfiguration

struct StreamSOCKSProxyVersion

struct PropertyKey

`NSStream` defines these string constants as keys for accessing stream properties using property(forKey:) and setting properties with setProperty(_:forKey:):

let NSStreamSocketSSLErrorDomain: String

The error domain used by `NSError` when reporting SSL errors.

let NSStreamSOCKSErrorDomain: String

The error domain used by `NSError` when reporting SOCKS errors.

