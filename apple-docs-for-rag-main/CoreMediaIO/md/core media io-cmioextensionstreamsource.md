

- Core Media I/O
-  CMIOExtensionStreamSource 

Protocol

# CMIOExtensionStreamSource

A protocol for objects that act as stream sources.

Mac Catalyst 15.4+macOS 12.3+

``` source
protocol CMIOExtensionStreamSource : NSObjectProtocol
```

## Overview

Create a class that adopts this protocol to configure stream properties and manage the stream life cycle.

## Topics

### Accessing the Source Format

var formats: [CMIOExtensionStreamFormat]

An array of formats that a stream supports.

**Required**

class CMIOExtensionStreamFormat

An object that describes the format of a media stream.

### Managing Stream Properties

var availableProperties: Set&lt;CMIOExtensionProperty>

A set of properties available for the stream.

**Required**

func streamProperties(forProperties: Set&lt;CMIOExtensionProperty>) throws -> CMIOExtensionStreamProperties

Gets the states of specified properties.

**Required**

func setStreamProperties(CMIOExtensionStreamProperties) throws

Sets the property state of a stream.

**Required**

### Managing a Stream

func authorizedToStartStream(for: CMIOExtensionClient) -> Bool

Determines whether to authorize an app to use this stream.

**Required**

func startStream() throws

Starts the stream of media data.

**Required**

func stopStream() throws

Stops the stream of media data.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Streams

class CMIOExtensionStream

An object that represents a stream of media data.

class CMIOExtensionStreamProperties

An object that describes the properties of an extension stream.

class CMIOExtensionClient

An object that represents a client of the extension.

