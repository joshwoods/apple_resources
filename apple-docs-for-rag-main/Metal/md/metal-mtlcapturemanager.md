

- Metal
-  MTLCaptureManager 

Class

# MTLCaptureManager

An instance you use to capture Metal command data in your app.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MTLCaptureManager
```

## Overview

Capture manager works with Metal’s frame capture feature to:

- Capture data about Metal commands programmatically. See Capturing a Metal workload programmatically.

- Filter captured commands to a specific MTLDevice, command queue, or capture scope.

- Assign a capture scope to use as the default when you click the camera button to invoke a frame capture from Xcode’s debug bar. See MTLCaptureScope.

The Metal debugger requires you to enable GPU Frame Capture in your project settings; see Capturing a Metal workload in Xcode.

Important

The capture manager records commands within MTLCommandBuffer objects that you create and commit while the capture session is active.

For more information about Metal frame capture, see Metal debugger.

## Topics

### Obtaining the Shared Capture Manager

class func shared() -> MTLCaptureManager

Provides the shared capture manager for your Metal app.

### Querying Support for a Capture Destination

func supportsDestination(MTLCaptureDestination) -> Bool

Checks to see whether a particular capture destination is supported.

### Creating a Capture Scope

func makeCaptureScope(device: any MTLDevice) -> any MTLCaptureScope

Creates a capture scope for commands submitted to a specific device object.

func makeCaptureScope(commandQueue: any MTLCommandQueue) -> any MTLCaptureScope

Creates a capture scope for commands submitted to a specific command queue.

var defaultCaptureScope: (any MTLCaptureScope)?

The capture scope to use when a capture is initiated in Xcode.

### Starting Capture

Start capturing Metal commands for presentation in the Metal debugger.

func startCapture(with: MTLCaptureDescriptor) throws

Starts capturing any of your app’s Metal commands, with the capture session defined by a descriptor object.

func startCapture(device: any MTLDevice)

Starts capturing any of your app’s Metal commands that are executed by the device object.

Deprecated

func startCapture(commandQueue: any MTLCommandQueue)

Starts capturing any of your app’s Metal commands that are executed by the command queue.

Deprecated

func startCapture(scope: any MTLCaptureScope)

Starts capturing any of your app’s Metal commands that are in the specified capture scope.

Deprecated

### Stopping Capture

func stopCapture()

Stops capturing Metal commands.

### Monitoring Capture

var isCapturing: Bool

A Boolean value that indicates whether Metal commands are being captured.

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

### Frame Capture

class MTLCaptureDescriptor

A configuration for a Metal capture session.

enum MTLCaptureDestination

The kinds of destinations for captured command data.

protocol MTLCaptureScope

A protocol that defines custom boundaries for a GPU frame capture.

