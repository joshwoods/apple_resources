

- Foundation
- Stream
-  Stream.Event 

Structure

# Stream.Event

Describes the constants that may be sent to the delegate as a bit field in the second parameter of stream(_:handle:) to specify the kind of stream event.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct Event
```

## Topics

### Constants

static var openCompleted: Stream.Event

The open has completed successfully.

static var hasBytesAvailable: Stream.Event

The stream has bytes to be read.

static var hasSpaceAvailable: Stream.Event

The stream can accept bytes for writing.

static var errorOccurred: Stream.Event

An error has occurred on the stream.

static var endEncountered: Stream.Event

The end of the stream has been reached.

static var openCompleted: Stream.Event

The open has completed successfully.

static var hasBytesAvailable: Stream.Event

The stream has bytes to be read.

static var hasSpaceAvailable: Stream.Event

The stream can accept bytes for writing.

static var errorOccurred: Stream.Event

An error has occurred on the stream.

static var endEncountered: Stream.Event

The end of the stream has been reached.

### Initializers

init(rawValue: UInt)

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

enum Status

The type declared for the constants listed in doc:stream/stream_status_constants.

Stream Status Constants

These constants indicate the current status of a stream. They are returned by streamStatus.

struct StreamNetworkServiceTypeValue

`NSStream` defines these string constants for specifying the service type of a stream.

struct StreamSOCKSProxyConfiguration

struct StreamSOCKSProxyVersion

struct StreamSocketSecurityLevel

`NSStream` defines these string constants for specifying the secure-socket layer (SSL) security level.

struct PropertyKey

`NSStream` defines these string constants as keys for accessing stream properties using property(forKey:) and setting properties with setProperty(_:forKey:):

let NSStreamSocketSSLErrorDomain: String

The error domain used by `NSError` when reporting SSL errors.

let NSStreamSOCKSErrorDomain: String

The error domain used by `NSError` when reporting SOCKS errors.

