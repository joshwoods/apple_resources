

- AVKit
-  AVPictureInPictureVideoCallViewController 

Class

# AVPictureInPictureVideoCallViewController

A view controller that presents content from a video call in Picture in Picture.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
class AVPictureInPictureVideoCallViewController
```

## Mentioned in 

Adopting Picture in Picture for video calls

## Overview

Important

The use of this API requires an entitlement. For information about requesting access, see com.apple.developer.avfoundation.multitasking-camera-access.

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

### Accessing the Active Call Presentation

var activeVideoCallSourceView: UIView?

The view that contains the video content of the call.

var activeVideoCallContentViewController: AVPictureInPictureVideoCallViewController

The view controller that presents the video call content.

