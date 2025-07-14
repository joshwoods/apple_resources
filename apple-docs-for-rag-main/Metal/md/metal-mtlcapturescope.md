

- Metal
-  MTLCaptureScope 

Protocol

# MTLCaptureScope

A protocol that defines custom boundaries for a GPU frame capture.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
protocol MTLCaptureScope : NSObjectProtocol
```

## Overview

A capture scope works with Metal’s frame capture feature to filter a captured frame to include the specific commands that you choose. By contrast, when you capture a frame with the default capture scope by clicking the camera button on Xcode’s debug bar, the resulting capture includes all the data from a single frame. You create your own capture scope when you want to choose which data Metal should record.

To determine exactly which Metal commands to record in a captured frame, call begin() and end() around the Metal calls you want the capture to include. In the case of a rendering loop, your calls to begin() and end() can capture a small part of a frame, or capture data across multiple frames.

You can use capture scopes in a few different ways:

- You can change Xcode’s default capturing behavior.

- In Xcode, you can add additional capture scopes that appear when you click and hold the camera button on the debug bar.

- You can programmatically trigger a capture session using a specific scope.

For more information about frame capture, see Metal debugger and Metal developer workflows. For more information on creating custom capture scopes, see Creating and using custom capture scopes.

## Topics

### Defining Capture Scope Boundaries

func begin()

Tells Metal to begin recording command information.

**Required**

func end()

Tells Metal to stop recording command information.

**Required**

### Identifying the Capture Scope

var label: String?

A string that identifies the capture scope.

**Required**

var device: any MTLDevice

The device object from which you created the capture scope.

**Required**

var commandQueue: (any MTLCommandQueue)?

The command queue that this capture scope uses to limit which commands are recorded.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Frame Capture

class MTLCaptureDescriptor

A configuration for a Metal capture session.

class MTLCaptureManager

An instance you use to capture Metal command data in your app.

enum MTLCaptureDestination

The kinds of destinations for captured command data.

