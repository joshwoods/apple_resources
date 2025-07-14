

- UIKit
-  UIScreen 

Class

# UIScreen

An object that defines the properties associated with a hardware-based display.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOS

``` source
@MainActor
class UIScreen
```

## Mentioned in 

Presenting content on a connected display

Building a desktop-class iPad app

## Overview

A UIScreen object provides information about the screens attached to an iOS, iPadOS, or tvOS device. A screen object for an iOS or iPadOS device has information about the integrated display or an attached display. A screen object for a tvOS device represents the television connected to the device. In a compatible iPad or iPhone app running in visionOS, don’t rely on screen-related properties to configure your app.

You don’t create any of these screen objects directly. Instead, fetch the screen object for one of your app’s windows from the UIWindowScene object that manages the window.

Avoid using screen objects to make decisions about your app’s interface. Use a screen object only as needed to retrieve screen-related information, such as the screen’s bounds rectangle, brightness, and overscan settings. Apps that rely on the screen dimensions can use the object in the fixedCoordinateSpace property as a fixed point of reference for any calculations they must make.

## Topics

### Getting the coordinate space

var coordinateSpace: any UICoordinateSpace

The current coordinate space of the screen.

var fixedCoordinateSpace: any UICoordinateSpace

The fixed coordinate space of the screen.

### Getting the size and scale

var bounds: CGRect

The bounding rectangle of the screen, measured in points.

var nativeBounds: CGRect

The bounding rectangle of the physical screen, measured in pixels.

var nativeScale: CGFloat

The native scale factor for the physical screen.

var scale: CGFloat

The natural scale factor associated with the screen.

### Managing brightness

var brightness: CGFloat

The brightness level of the screen.

var wantsSoftwareDimming: Bool

A Boolean value that indicates whether the screen may be dimmed lower than the hardware is normally capable of by emulating it in software.

### Managing screen modes

var currentMode: UIScreenMode?

The current screen mode associated with the screen.

var preferredMode: UIScreenMode?

The preferred display mode for the screen.

var availableModes: [UIScreenMode]

The display modes that can be associated with the screen.

### Managing overscan compensation

var overscanCompensationInsets: UIEdgeInsets

The edge inset values needed to avoid clipping the rectangle.

var overscanCompensation: UIScreen.OverscanCompensation

For an external screen, this property sets the desired technique to compensate for overscan.

enum OverscanCompensation

Describes different techniques for compensating for pixel loss at the edge of the screen.

### Getting the calibrated latency

var calibratedLatency: CFTimeInterval

The user-calibrated latency for the current screen.

### Getting the reference display mode status

var referenceDisplayModeStatus: UIScreen.ReferenceDisplayModeStatus

The status of the screen’s reference display mode.

enum ReferenceDisplayModeStatus

Describes a screen’s reference display mode status.

var currentEDRHeadroom: CGFloat

The screen’s current headroom when displaying extended dynamic range content.

var potentialEDRHeadroom: CGFloat

The screen’s maximum headroom when displaying extended dynamic range content.

### Getting a display link

func displayLink(withTarget: Any, selector: Selector) -> CADisplayLink?

Returns a display link object for the current screen.

var maximumFramesPerSecond: Int

The maximum number of frames per second a screen can render.

### Capturing a snapshot

func snapshotView(afterScreenUpdates: Bool) -> UIView

Returns a snapshot view based on the current screen contents.

### Detecting screen capture

var isCaptured: Bool

A Boolean value that indicates whether the system is actively cloning the screen to another destination.

Deprecated

var mirrored: UIScreen?

The screen an external display mirrors from.

### Notifications

class let brightnessDidChangeNotification: NSNotification.Name

A notification that posts when a screen’s brightness changes.

class let modeDidChangeNotification: NSNotification.Name

A notification that posts when a screen’s mode changes.

class let capturedDidChangeNotification: NSNotification.Name

A notification that posts when the capture status of a screen changes.

class let referenceDisplayModeStatusDidChangeNotification: NSNotification.Name

A notification that posts when there’s a change to a screen’s reference display mode status.

### Deprecated

Deprecated symbols

Review unsupported symbols and their replacements.

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
- Sendable
- UITraitEnvironment

## See Also

### Screens

Presenting content on a connected display

Fill connected displays with additional content from your app.

class UIScreenMode

A possible set of attributes that can apply to a screen object.

