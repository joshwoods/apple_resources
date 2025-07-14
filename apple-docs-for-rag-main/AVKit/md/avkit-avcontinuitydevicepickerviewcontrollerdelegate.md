

- AVKit
-  AVContinuityDevicePickerViewControllerDelegate 

Protocol

# AVContinuityDevicePickerViewControllerDelegate

An interface that responds to events from a continuity device picker view controller.

tvOS 9.0+

``` source
protocol AVContinuityDevicePickerViewControllerDelegate : NSObjectProtocol
```

## Overview

Your app can respond to the various outcome events from an AVContinuityDevicePickerViewController instance with the following steps:

1.  Adopt the AVContinuityDevicePickerViewControllerDelegate protocol with one of the app’s classes.

2.  Create an instance of that class.

3.  Assign that instance to the view controller’s delegate property.

## Topics

### Responding to continuity device events

func continuityDevicePickerWillBeginPresenting(AVContinuityDevicePickerViewController)

Informs the delegate that a continuity device picker is about to present its UI so that a person can select and connect a continuity device.

func continuityDevicePickerDidCancel(AVContinuityDevicePickerViewController)

Informs the delegate when a person declines to select a continuity device by dismissing an app’s continuity device picker.

func continuityDevicePicker(AVContinuityDevicePickerViewController, didConnect: AVContinuityDevice)

Informs the delegate when a person selects and connects a continuity device to the system with a continuity device picker.

func continuityDevicePickerDidEndPresenting(AVContinuityDevicePickerViewController)

Informs the delegate that a continuity device picker is no longer presenting its UI to a person.

## Relationships

### Inherits From

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

class AVDisplayManager

A tvOS management object that controls whether a TV switches modes to match the video’s native mode.

class AVContinuityDevicePickerViewController

A view controller that provides an interface to a person so they can select and connect a continuity device to the system.

