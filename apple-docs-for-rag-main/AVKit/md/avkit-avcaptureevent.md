

- AVKit
-  AVCaptureEvent 

Class

# AVCaptureEvent

An object that describes a user interaction with a system hardware button.

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+

``` source
class AVCaptureEvent
```

## Overview

Inspect a capture event’s phase to determine whether the event begins, ends, or is in a canceled state.

## Topics

### Inspecting the event

var phase: AVCaptureEventPhase

The current phase of a capture event.

enum AVCaptureEventPhase

Constants that indicate the phase of a system capture event.

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

### iOS Playback and Capture

Playing video content in a standard user interface

Play media full screen, embedded inline, or in a floating Picture in Picture (PiP) window using a player view controller.

class AVPlayerViewController

A view controller that displays content from a player and presents a native user interface to control playback.

protocol AVPlayerViewControllerDelegate

A protocol that defines the methods to implement to respond to player view controller events.

class AVCaptureEventInteraction

An object that registers handlers to respond to capture events from system hardware buttons.

