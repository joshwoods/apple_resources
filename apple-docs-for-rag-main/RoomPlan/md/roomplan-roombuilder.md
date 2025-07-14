

- RoomPlan
-  RoomBuilder 

Class

# RoomBuilder

An object that generates a 3D asset from room-capture data.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
class RoomBuilder
```

## Overview

This class processes data from an earlier scan to generate a detailed CapturedRoom object.

Your app receives raw captured room data (CapturedRoomData) through:

- The view delegate (RoomCaptureViewDelegate) callback captureView(shouldPresent:error:) for an app that provides room-scanning features through the framework-provided view (RoomCaptureView).

- The scan session (RoomCaptureSession) callback captureSession(_:didEndWith:error:) for an app that provides room-scanning features by displaying its own view.

Your app generates a detailed captured room object by calling capturedRoom(from:) on the raw data. Your app can then inspect or modify this data before exporting the scanned room to a USDZ file.

## Topics

### Creating a room builder

init(options: RoomBuilder.ConfigurationOptions)

Creates a session with assets from RSCaptureSession

struct ConfigurationOptions

The configuration options for the RoomBuilder

### Processing a prior scan

func capturedRoom(from: CapturedRoomData) async throws -> CapturedRoom

Processes the specified raw scan results and returns a detailed representation of the room.

### Handling errors

enum BuildError

Errors that can occur during captured room-data processing.

## See Also

### 3D Asset Output

Providing custom models for captured rooms and structure exports

Enhance the look of an exported 3D model by substituting object bounding boxes with detailed 3D renditions.

class StructureBuilder

An object that combines multiple scan sessions into a single captured result.

struct USDExportOptions

Options that determine the underlying data format of a scan export.

