

- AVKit
-  AVDisplayManager 

Class

# AVDisplayManager

A tvOS management object that controls whether a TV switches modes to match the video’s native mode.

tvOS 11.2+visionOS 1.0+

``` source
class AVDisplayManager
```

## Overview

If you set the display manager’s preferredDisplayCriteria, when a user enables a Match Content setting, the TV attempts to change modes to match the currently playing video’s native display criteria.

Important

Don’t directly instantiate a display manager object. Instead, access the current instance from the key window’s avDisplayManager property.

## Topics

### Matching a Video’s Native Display Mode

var preferredDisplayCriteria: AVDisplayCriteria?

A hint for the TV to set the display mode to best match the currently playing content’s display criteria.

var isDisplayCriteriaMatchingEnabled: Bool

A Boolean value that indicates whether the user has enabled display critera matching.

var isDisplayModeSwitchInProgress: Bool

A Boolean value that indicates whether a display mode switch is in progress.

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

### tvOS Playback and Capture

Customizing the tvOS Playback Experience

Adopt the latest features of the redesigned tvOS player user interface to provide a more streamlined way to watch your content.

Presenting Navigation Markers

Present navigation markers in the Chapters panel to help users quickly navigate your content.

Working with Interstitial Content

Present additional content alongside your main media presentation using HTTP Live Streaming support.

Presenting Content Proposals in tvOS

Display a preview of an upcoming media item at the conclusion of the currently playing media item.

Working with Overlays and Parental Controls in tvOS

Add interactive overlays, parental controls, and livestream channel flipping using a player view controller.

Supporting Continuity Camera in your tvOS app

Capture high-quality photos, video, and audio in your Apple TV app by connecting an iPhone or iPad as a continuity device.

class AVPlayerViewController

A view controller that displays content from a player and presents a native user interface to control playback.

protocol AVPlayerViewControllerDelegate

A protocol that defines the methods to implement to respond to player view controller events.

class AVInterstitialTimeRange

A time range in an audiovisual presentation for content with an interstitial designation, such as advertisements or legal notices.

class AVNavigationMarkersGroup

A set of markers for navigating playback of an audiovisual presentation.

class AVContentProposalViewController

A view controller that proposes content to watch next.

class AVContinuityDevicePickerViewController

A view controller that provides an interface to a person so they can select and connect a continuity device to the system.

protocol AVContinuityDevicePickerViewControllerDelegate

An interface that responds to events from a continuity device picker view controller.

