

- AVKit
-  AVPlayerViewControllerDelegate 

Protocol

# AVPlayerViewControllerDelegate

A protocol that defines the methods to implement to respond to player view controller events.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
protocol AVPlayerViewControllerDelegate : NSObjectProtocol
```

## Mentioned in 

Working with Interstitial Content

Adopting Picture in Picture in a Standard Player

Presenting Content Proposals in tvOS

## Topics

### Dismissing the Player View Controller

func playerViewControllerShouldDismiss(AVPlayerViewController) -> Bool

Asks the delegate object whether the player view controller dismisses itself upon request.

func playerViewControllerWillBeginDismissalTransition(AVPlayerViewController)

Tells the delegate when the player view controller is about to start its dismissal transition.

func playerViewControllerDidEndDismissalTransition(AVPlayerViewController)

Tells the delegate when the player view controller ends its dismissal transition.

### Responding to Picture in Picture Life Cycle Events

func playerViewControllerShouldAutomaticallyDismissAtPictureInPictureStart(AVPlayerViewController) -> Bool

Asks the delegate whether the player view controller automatically dismisses itself when Picture in Picture starts.

func playerViewControllerWillStartPictureInPicture(AVPlayerViewController)

Tells the delegate when Picture in Picture is about to start.

func playerViewControllerDidStartPictureInPicture(AVPlayerViewController)

Tells the delegate when Picture in Picture starts.

func playerViewController(AVPlayerViewController, failedToStartPictureInPictureWithError: any Error)

Tells the delegate when Picture in Picture fails to start.

func playerViewControllerWillStopPictureInPicture(AVPlayerViewController)

Tells the delegate when Picture in Picture is about to stop.

func playerViewControllerDidStopPictureInPicture(AVPlayerViewController)

Tells the delegate when Picture in Picture stops.

func playerViewController(AVPlayerViewController, restoreUserInterfaceForPictureInPictureStopWithCompletionHandler: (Bool) -> Void)

Tells the delegate when Picture in Picture is about to stop so you can restore your app’s user interface.

### Responding to Navigation Events

func playerViewController(AVPlayerViewController, timeToSeekAfterUserNavigatedFrom: CMTime, to: CMTime) -> CMTime

Tells the delegate when the user skips, scrubs, or otherwise navigates to a new time and wants to resume playback at the target time.

func playerViewController(AVPlayerViewController, willResumePlaybackAfterUserNavigatedFrom: CMTime, to: CMTime)

Tells the delegate when the user navigates to a new time and playback is about to begin.

func skipToPreviousItem(for: AVPlayerViewController)

Tells the delegate when the user requests skipping to the previous item in the timeline.

func skipToNextItem(for: AVPlayerViewController)

Tells the delegate when the user requests skipping to the next item in the timeline.

### Responding to Interstitial Content Playback Events

func playerViewController(AVPlayerViewController, willPresent: AVInterstitialTimeRange)

Tells the delegate when the player view controller is about to start playing a range of interstitial content.

func playerViewController(AVPlayerViewController, didPresent: AVInterstitialTimeRange)

Tells the delegate when the player view controller finishes playing a range of interstitial content.

### Responding to Content Proposals

func playerViewController(AVPlayerViewController, shouldPresent: AVContentProposal) -> Bool

Asks the delegate whether the player view controller presents a content proposal.

func playerViewController(AVPlayerViewController, didAccept: AVContentProposal)

Tells the delegate when the user accepts the proposed content.

func playerViewController(AVPlayerViewController, didReject: AVContentProposal)

Tells the delegate when the user rejects the proposed content.

### Responding to Media Selection

func playerViewController(AVPlayerViewController, didSelect: AVMediaSelectionOption?, in: AVMediaSelectionGroup)

Tells the delegate when the user selects a media option from a media selection group.

### Responding to Transport Bar Changes

func playerViewController(AVPlayerViewController, willTransitionToVisibilityOfTransportBar: Bool, with: any AVPlayerViewControllerAnimationCoordinator)

Tells the delegate when the transport bar’s visibility is about to change.

protocol AVPlayerViewControllerAnimationCoordinator

A protocol that defines the methods to implement to synchronize animations with playback controls’ visibility animation.

### Responding to Channel Changes

func playerViewController(AVPlayerViewController, skipToNextChannel: (Bool) -> Void)

Tells the delegate when the user wants to skip to the next channel.

func playerViewController(AVPlayerViewController, skipToPreviousChannel: (Bool) -> Void)

Tells the delegate when the user wants to skip to the previous channel.

func nextChannelInterstitialViewController(for: AVPlayerViewController) -> UIViewController

Asks the delegate for a view controller that describes the layout of the next channel’s interstitial view.

func previousChannelInterstitialViewController(for: AVPlayerViewController) -> UIViewController

Asks the delegate for a view controller that describes the layout of the previous channel’s interstitial view.

### Responding to Full-Screen Presentations

func playerViewController(AVPlayerViewController, willBeginFullScreenPresentationWithAnimationCoordinator: any UIViewControllerTransitionCoordinator)

Tells the delegate when the player view controller is about to start full-screen display.

func playerViewController(AVPlayerViewController, willEndFullScreenPresentationWithAnimationCoordinator: any UIViewControllerTransitionCoordinator)

Tells the delegate when the player view controller is about to end full-screen display.

func playerViewController(AVPlayerViewController, restoreUserInterfaceForFullScreenExitWithCompletionHandler: (Bool) -> Void)

Tells the delegate to restore the app’s user interface after returning from a full-screen presentation.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### iOS Playback and Capture

Playing video content in a standard user interface

Play media full screen, embedded inline, or in a floating Picture in Picture (PiP) window using a player view controller.

class AVPlayerViewController

A view controller that displays content from a player and presents a native user interface to control playback.

class AVCaptureEventInteraction

An object that registers handlers to respond to capture events from system hardware buttons.

class AVCaptureEvent

An object that describes a user interaction with a system hardware button.

