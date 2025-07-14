

- RoomPlan
-  RoomCaptureViewDelegate 

Protocol

# RoomCaptureViewDelegate

A specification to post-process the results of a scan.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
protocol RoomCaptureViewDelegate : NSCoding
```

## Overview

The room-capture view’s delegate property (delegate) is of this type.

When your app scans a room using the framework-provided view (RoomCaptureView), your delegate receives the raw scan results through the `roomDataForProcessing` argument of captureView(shouldPresent:error:).

If your app returns `true` to captureView(shouldPresent:error:), the framework processes the raw results and calls captureView(didPresent:error:) when processing completes.

## Topics

### Post-processing scan results

func captureView(shouldPresent: CapturedRoomData, error: (any Error)?) -> Bool

Indicates whether the app processes raw scan results immediately after a scan session stops.

**Required** Default implementation provided.

func captureView(didPresent: CapturedRoom, error: (any Error)?)

Provides the delegate with the processed scan results as the view presents them.

**Required** Default implementation provided.

### Default implementations

func captureView(shouldPresent: CapturedRoomData, error: (any Error)?) -> Bool

Indicates that the app receives and displays post-processed scan results when the scan session stops.

func captureView(didPresent: CapturedRoom, error: (any Error)?)

Provides the delegate with the post-processed scan results once the view presents them.

## Relationships

### Inherits From

- NSCoding

## See Also

### User Interface

class RoomCaptureView

A view that enables the user to scan their room with the device’s camera.

