

- RoomPlan
-  CapturedRoomData 

Structure

# CapturedRoomData

An opaque object that holds the raw results of a scan.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
struct CapturedRoomData
```

## Overview

When your app completes a scan session by calling stop(), the framework provides your app with raw scan results in one of the following ways:

- The captureView(shouldPresent:error:) callback for an app that scans rooms using the framework-provided view (RoomCaptureView)

- The captureSession(_:didEndWith:error:) callback for an app that implements its own room-scanning view

With an instance of this structure, your app can:

- Process the raw data into a detailed captured room object (CapturedRoom) by creating a room builder (RoomBuilder) and calling its capturedRoom(from:) function.

- Serialize to an encoder object, for example, to defer processing to a later date or to defer processing to another device.

## Topics

### Deserializing a prior scan

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Serializing a prior scan

func encode(to: any Encoder) throws

Serializes captured room data to the specified encoder.

## Relationships

### Conforms To

- Decodable
- Encodable
- Sendable

## See Also

### Captured Data

Merging multiple scans into a single structure

Export a 3D model that consists of multiple rooms captured in the same physical vicinity.

Scanning the rooms of a single structure

Create an AR experience that enables people to scan a building that contains multiple rooms.

struct CapturedRoom

A structure that provides the key details of a scanned room.

struct CapturedStructure

An object that holds the results of the merger of multiple capture sessions.

Captured Object Attributes

Determine details about the objects and surfaces that the framework identifies in a scan.

