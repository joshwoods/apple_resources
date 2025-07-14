

- RoomPlan
-  RoomCaptureView 

Class

# RoomCaptureView

A view that enables the user to scan their room with the device’s camera.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
@MainActor @objc @preconcurrency
class RoomCaptureView
```

## Mentioned in 

Scanning the rooms of a single structure

## Overview

This class provides your app with a view that manages the scan process from start to finish, including:

- A camera feed that users look through to see their room in AR.

- Real-time graphic overlays that display on top of physical structures in the room to convey scanning progress.

- User instructions that explain how to position the device, if the framework requires a specific kind of device movement or perspective to complete the capture.

When the app determines that the current scan is complete, the view displays a small-scale version of the scanned room for the user to approve.

Alternatively, your app can display custom graphics during the scanning process by creating and using a scan session object (RoomCaptureSession) directly.

See Create a 3D model of an interior room by guiding the user through an AR experience for a sample code project that demonstrates `RoomCaptureView`.

## Topics

### Creating a room-capture view

init(frame: CGRect, arSession: ARSession)

Creates a room-capture view with the given AR session.

init(frame: CGRect)

Creates a view that sizes to the specified frame.

init?(coder: NSCoder)

Creates a view by deserializing from the specified coder.

### Reacting to scan events

var captureSession: RoomCaptureSession!

An object that notifies a delegate of particular events in the room-scanning life cycle.

var delegate: (any RoomCaptureViewDelegate)?

An object that determines whether to post-process the results of a scan.

### Displaying scan progress

var isModelEnabled: Bool

A Boolean value that determines whether the view displays a miniature rendering of the scanned room at the bottom of its bounds.

### Accessing view features

var subviews: [UIView]

An array that contains the view’s subviews.

func layoutSubviews()

Instructs the view’s subviews to position within the view.

func encode(with: NSCoder)

Serializes the view to the specified coder.

func traitCollectionDidChange(UITraitCollection?)

Notifies the view when the device orientation changes.

## Relationships

### Inherits From

- UIView

### Conforms To

- CALayerDelegate
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSTouchBarProvider
- UIAccessibilityIdentification
- UIActivityItemsConfigurationProviding
- UIAppearance
- UIAppearanceContainer
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### User Interface

protocol RoomCaptureViewDelegate

A specification to post-process the results of a scan.

