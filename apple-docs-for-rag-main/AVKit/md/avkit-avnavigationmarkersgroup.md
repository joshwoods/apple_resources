

- AVKit
-  AVNavigationMarkersGroup 

Class

# AVNavigationMarkersGroup

A set of markers for navigating playback of an audiovisual presentation.

tvOS 9.0+

``` source
class AVNavigationMarkersGroup
```

## Mentioned in 

Presenting Navigation Markers

## Overview

The most common form of a navigation markers group is a chapter list; however, you can also provide other sets of markers to allow a user to jump to significant events in the presentation. For example, a “Goals Scored” markers group might summarize key moments in a recorded sporting event. When you associate navigation markers with an AVPlayerItem object you present with an AVPlayerViewController, the user interface provides options for navigating each group.

## Topics

### Creating a Navigation Marker Group

init(title: String?, timedNavigationMarkers: [AVTimedMetadataGroup])

Initializes a navigation markers group with the specified title and array of timed navigation markers.

init(title: String?, dateRangeNavigationMarkers: [AVDateRangeMetadataGroup])

Initializes a navigation markers group with the specified title and array of date range navigation markers.

### Inspecting Navigation Metadata

var title: String?

The title of the marker group.

var timedNavigationMarkers: [AVTimedMetadataGroup]?

The array of timed navigation markers for which the group provides navigation.

var dateRangeNavigationMarkers: [AVDateRangeMetadataGroup]?

The array of date range navigation markers for which the group provides navigation.

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

class AVContentProposalViewController

A view controller that proposes content to watch next.

class AVDisplayManager

A tvOS management object that controls whether a TV switches modes to match the video’s native mode.

class AVContinuityDevicePickerViewController

A view controller that provides an interface to a person so they can select and connect a continuity device to the system.

protocol AVContinuityDevicePickerViewControllerDelegate

An interface that responds to events from a continuity device picker view controller.

