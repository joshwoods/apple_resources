

- Media Player
-  MPMediaPickerController 

Class

# MPMediaPickerController

A specialized view controller that provides a graphical interface for selecting media items.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+

``` source
@MainActor
class MPMediaPickerController
```

## Overview

An MPMediaPickerController object, or media item picker, is a specialized view controller that you employ to provide a graphical interface for selecting media items. To display a media item picker, present it modally on an existing view controller. Presenting an MPMediaPickerController in non-modal mode; for example, pushing a MPMediaPickerController onto an existing UINavigationController stack causes your app to crash. MPMediaItem describes media items.

To respond to user selections and to dismiss a media item picker, use the MPMediaPickerControllerDelegate protocol.

Notes

The MPMediaPickerController class supports portrait mode only. This class doesn’t support subclassing, and don’t modify the view hierarchy, which is private. In a compatible iPad or iPhone app in visionOS, presenting this picker displays an alert notifying the person that picking media items isn’t supported.

## Topics

### Initializing a media item picker

init

Initializes a media item picker for all media types.

init(mediaTypes: MPMediaType)

Initializes a media item picker for specified media types.

### Responding to media item picker selections

var delegate: (any MPMediaPickerControllerDelegate)?

The delegate for a media item picker.

protocol MPMediaPickerControllerDelegate

The protocol you implement so that a media item picker can respond to a user making media item selections.

### Using a media item picker

var allowsPickingMultipleItems: Bool

A Boolean value specifying the default selection behavior for a media item picker.

var showsCloudItems: Bool

A Boolean value specifying whether to display iCloud Media Library items for a media picker.

var mediaTypes: MPMediaType

The media types that media item picker presents.

var prompt: String?

A prompt, for the user, that appears above the navigation bar buttons.

var showsItemsWithProtectedAssets: Bool

A Boolean value that specifies whether the media item picker displays protected assets.

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

### Media player user interface

Displaying a media picker from your app

Let users choose the music they want to play by displaying a media picker interface from within your app.

class MPVolumeView

A slider control for setting the system audio output volume, and a button for choosing the audio output route.

