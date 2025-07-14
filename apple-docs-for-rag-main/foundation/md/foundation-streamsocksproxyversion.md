

- Foundation
-  StreamSOCKSProxyVersion 

Structure

# StreamSOCKSProxyVersion

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct StreamSOCKSProxyVersion
```

## Topics

### Type Properties

static let version4: StreamSOCKSProxyVersion

Possible value for `NSStreamSOCKSProxyVersionKey`.

static let version5: StreamSOCKSProxyVersion

Possible value for `NSStreamSOCKSProxyVersionKey`.

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

struct StreamSocketSecurityLevel

`NSStream` defines these string constants for specifying the secure-socket layer (SSL) security level.

struct PropertyKey

`NSStream` defines these string constants as keys for accessing stream properties using property(forKey:) and setting properties with setProperty(_:forKey:):

let NSStreamSocketSSLErrorDomain: String

The error domain used by `NSError` when reporting SSL errors.

let NSStreamSOCKSErrorDomain: String

The error domain used by `NSError` when reporting SOCKS errors.

