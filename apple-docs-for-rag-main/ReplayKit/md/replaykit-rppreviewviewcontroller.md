

- ReplayKit
-  RPPreviewViewController 

Class

# RPPreviewViewController

An object that displays a user interface where users preview and edit a screen recording that you create with ReplayKit.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 11.0+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
class RPPreviewViewController
```

## Overview

Upon completion of a successful recording, the preview view controller is passed into the completion handler for stopRecording(handler:).

## Topics

### Displaying the Preview UI

var mode: RPPreviewViewControllerMode

The type of screen that appears when the view is presented.

enum RPPreviewViewControllerMode

The modes used to determine whether the preview view controller or the share screen appears when editing a replay.

var previewControllerDelegate: (any RPPreviewViewControllerDelegate)?

The preview view controller’s delegate.

protocol RPPreviewViewControllerDelegate

The protocol you implement to respond to changes to a screen-recording user interface.

## Relationships

### Inherits From

- NSViewController
- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSEditor
- NSExtensionRequestHandling
- NSObjectProtocol
- NSSeguePerforming
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- Sendable
- UIActivityItemsConfigurationProviding
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIStateRestoring
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Replay Sharing

Recording and Streaming Your macOS App

Share screen recordings, or broadcast live audio and video of your app, by adding ReplayKit to your macOS apps and games.

class RPScreenRecorder

The shared recorder object that provides the ability to record audio and video of your app.

