

- ScreenCaptureKit
-  SCStream 

Class

# SCStream

An instance that represents a stream of shareable content.

Mac Catalyst 18.2+macOS 12.3+

``` source
class SCStream
```

## Overview

Use a stream to capture video of screen content like apps and windows. Create a content stream by passing it an instance of SCContentFilter and an SCStreamConfiguration object. The stream uses the filter to determine which screen content to capture, and uses the configuration data to configure the output.

## Topics

### Creating a stream

init(filter: SCContentFilter, configuration: SCStreamConfiguration, delegate: (any SCStreamDelegate)?)

Creates a stream with a content filter and configuration.

### Updating stream configuration

func updateConfiguration(SCStreamConfiguration, completionHandler: (((any Error)?) -> Void)?)

Updates the stream with a new configuration.

func updateContentFilter(SCContentFilter, completionHandler: (((any Error)?) -> Void)?)

Updates the stream by applying a new content filter.

### Adding and removing stream output

func addStreamOutput(any SCStreamOutput, type: SCStreamOutputType, sampleHandlerQueue: dispatch_queue_t?) throws

Adds a destination that receives the stream output.

func removeStreamOutput(any SCStreamOutput, type: SCStreamOutputType) throws

Removes a destination from receiving stream output.

### Adding and removing recording output

func addRecordingOutput(SCRecordingOutput) throws

func removeRecordingOutput(SCRecordingOutput) throws

class SCRecordingOutput

### Starting and stopping a stream

func startCapture(completionHandler: (((any Error)?) -> Void)?)

Starts the stream with a callback to indicate whether it successfully starts.

func stopCapture(completionHandler: (((any Error)?) -> Void)?)

Stops the stream.

### Stream synchronization

var synchronizationClock: CMClock?

A clock to use for output synchronization.

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

### Content capture

class SCStreamConfiguration

An instance that provides the output configuration for a stream.

class SCContentFilter

An instance that filters the content a stream captures.

protocol SCStreamDelegate

A delegate protocol your app implements to respond to stream events.

class SCScreenshotManager

An instance for the capture of single frames from a stream.

