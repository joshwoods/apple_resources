

- Foundation
-  StreamDelegate 

Protocol

# StreamDelegate

An interface that delegates of a stream instance use to handle events on the stream.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol StreamDelegate : NSObjectProtocol
```

## Mentioned in 

Uploading streams of data

## Topics

### Using Streams

func stream(Stream, handle: Stream.Event)

The delegate receives this message when a given event has occurred on a given stream.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Streams

class Stream

An abstract class representing a stream.

class InputStream

A stream that provides read-only stream functionality.

class OutputStream

A stream that provides write-only stream functionality.

