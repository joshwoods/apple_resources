

- UIKit
-  UIVideoEditorController 

Class

# UIVideoEditorController

A view controller that manages the system interface for trimming video frames and encoding a previously recorded movie.

iOS 3.1+iPadOS 3.1+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UIVideoEditorController
```

## Overview

A video editor manages user interactions and provides the filesystem path of the edited movie to your delegate object (see UIVideoEditorControllerDelegate). The features of the UIVideoEditorController class are available only on devices that support video recording. Use a video editor when your intent is to provide an interface for movie editing. While the UIImagePickerController class also lets a user trim movies, its primary roles are choosing saved pictures and movies, and capturing new pictures and movies.

Important

The `UIVideoEditorController` class supports portrait mode only. This class is intended to be used as-is and doesn’t support subclassing. The view hierarchy for this class is private; don’t modify the view hierarchy. This class doesn’t support modifications to its appearance by use of overlay views.

## Topics

### Managing changes to the video

var delegate: (any UINavigationControllerDelegate &amp; UIVideoEditorControllerDelegate)?

The video editor’s delegate object.

protocol UIVideoEditorControllerDelegate

A set of methods that your delegate object must implement to respond to the video editor.

### Determining editing availability

class func canEditVideo(atPath: String) -> Bool

Returns a Boolean value indicating whether a video file can be edited.

### Configuring the editor

var videoMaximumDuration: TimeInterval

The maximum duration, in seconds, permitted for trimmed movies saved by the video editor.

var videoPath: String

The filesystem path to the movie to be loaded by the video editor.

var videoQuality: UIImagePickerController.QualityType

The video quality to use when saving a trimmed movie.

## Relationships

### Inherits From

- UINavigationController

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

### Images and video

class UIImagePickerController

A view controller that manages the system interfaces for taking pictures, recording movies, and choosing items from the user’s media library.

