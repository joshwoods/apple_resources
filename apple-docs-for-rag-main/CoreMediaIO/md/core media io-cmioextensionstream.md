

- Core Media I/O
-  CMIOExtensionStream 

Class

# CMIOExtensionStream

An object that represents a stream of media data.

Mac Catalyst 15.4+macOS 12.3+

``` source
class CMIOExtensionStream
```

## Mentioned in 

Creating a camera extension with Core Media I/O

## Overview

A stream delivers media samples to or from a CMIOExtensionDevice.

## Topics

### Creating a Stream

init(localizedName: String, streamID: UUID, direction: CMIOExtensionStream.Direction, clockType: CMIOExtensionStream.ClockType, source: any CMIOExtensionStreamSource)

Creates a stream.

init(localizedName: String, streamID: UUID, direction: CMIOExtensionStream.Direction, customClockConfiguration: CMIOExtensionStreamCustomClockConfiguration, source: any CMIOExtensionStreamSource)

Creates a stream that uses a custom clock configuration.

### Identifying a Stream

var localizedName: String

A localized name for the stream.

var streamID: UUID

A universally unique identifier for the stream.

### Accessing Clients

var streamingClients: [CMIOExtensionClient]

An array of clients of the stream.

### Inspecting a Stream

var source: (any CMIOExtensionStreamSource)?

The source object for the stream.

var direction: CMIOExtensionStream.Direction

The data-flow direction of the stream.

enum Direction

Constants that define the data-flow direction of the stream.

var clockType: CMIOExtensionStream.ClockType

A clock type for the stream.

enum ClockType

Constants that indicate the clock type of a stream.

var customClockConfiguration: CMIOExtensionStreamCustomClockConfiguration?

An optional custom clock configuration for a stream.

class CMIOExtensionStreamCustomClockConfiguration

An object that describes the parameters to create a custom clock on the host side.

### Processing Data

func consumeSampleBuffer(from: CMIOExtensionClient, completionHandler: (CMSampleBuffer?, UInt64, CMIOExtensionStream.DiscontinuityFlags, Bool, (any Error)?) -> Void)

Consumes a sample buffer from a client.

func send(CMSampleBuffer, discontinuity: CMIOExtensionStream.DiscontinuityFlags, hostTimeInNanoseconds: UInt64)

Sends a media sample to stream client.

struct DiscontinuityFlags

Constants that specify the types of discontinuities that can occur in a media stream.

### Posting Property Changes

func notifyPropertiesChanged([CMIOExtensionProperty : CMIOExtensionPropertyState&lt;AnyObject>])

Notifies clients about stream property changes.

### Managing Scheduled Output

func notifyScheduledOutputChanged(CMIOExtensionScheduledOutput)

Notifies clients when a particular buffer is output.

class CMIOExtensionScheduledOutput

An object that represents scheduled output.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Streams

protocol CMIOExtensionStreamSource

A protocol for objects that act as stream sources.

class CMIOExtensionStreamProperties

An object that describes the properties of an extension stream.

class CMIOExtensionClient

An object that represents a client of the extension.

