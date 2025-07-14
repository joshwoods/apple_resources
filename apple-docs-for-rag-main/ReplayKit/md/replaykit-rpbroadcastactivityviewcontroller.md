

- ReplayKit
-  RPBroadcastActivityViewController 

Class

# RPBroadcastActivityViewController

A view controller that displays a user interface where users choose a broadcast service.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
class RPBroadcastActivityViewController
```

## Overview

The view controller displays the broadcast services currently installed on the device. On iPad, you must present the broadcast activity view controller as a popover.

## Topics

### Presenting the Broadcast Activity UI

class func load(handler: (RPBroadcastActivityViewController?, (any Error)?) -> Void)

Loads a broadcast activity view controller.

class func load(withPreferredExtension: String?, handler: (RPBroadcastActivityViewController?, (any Error)?) -> Void)

Loads a broadcast activity view controller with a preferred extension.

### Getting the Delegate

var delegate: (any RPBroadcastActivityViewControllerDelegate)?

The delegate for the broadcast activity view controller.

protocol RPBroadcastActivityViewControllerDelegate

The protocol you implement to respond to changes to a broadcast activity user interface.

## Relationships

### Inherits From

- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSExtensionRequestHandling
- NSObjectProtocol
- NSTouchBarProvider
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

### Live Broadcast Implementation

class RPSystemBroadcastPickerView

A view displaying a broadcast button that, when tapped, shows a broadcast picker.

class RPBroadcastActivityController

A controller object that presents the macOS broadcast picker.

protocol RPBroadcastActivityControllerDelegate

A protocol that defines the methods to implement to respond to selection events from a broadcast activity controller.

class RPBroadcastConfiguration

An object used to configure the movie clips produced during a live broadcast.

Deprecated

