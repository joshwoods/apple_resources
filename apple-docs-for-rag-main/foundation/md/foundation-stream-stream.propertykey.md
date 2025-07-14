

- Foundation
- Stream
-  Stream.PropertyKey 

Structure

# Stream.PropertyKey

`NSStream` defines these string constants as keys for accessing stream properties using property(forKey:) and setting properties with setProperty(_:forKey:):

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct PropertyKey
```

## Topics

### Type Properties

static let dataWrittenToMemoryStreamKey: Stream.PropertyKey

Value is an `NSData` instance containing the data written to a memory stream.

static let fileCurrentOffsetKey: Stream.PropertyKey

Value is an `NSNumber` object containing the current absolute offset of the stream.

static let networkServiceType: Stream.PropertyKey

The type of service for the stream. Providing the service type allows the system to properly handle certain attributes of the stream, including routing and suspension behavior. Most streams do not need to set this property. See `Stream Service Types` for a list of possible values.

static let socketSecurityLevelKey: Stream.PropertyKey

static let socksProxyConfigurationKey: Stream.PropertyKey

Value is an `NSDictionary` object containing SOCKS proxy configuration information.

### Initializers

init(String)

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

struct StreamSocketSecurityLevel

`NSStream` defines these string constants for specifying the secure-socket layer (SSL) security level.

let NSStreamSocketSSLErrorDomain: String

The error domain used by `NSError` when reporting SSL errors.

let NSStreamSOCKSErrorDomain: String

The error domain used by `NSError` when reporting SOCKS errors.

