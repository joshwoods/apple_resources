

- AVKit
- AVPlayerViewController
-  customOverlayViewController 

Instance Property

# customOverlayViewController

A view controller that presents custom content over the player view.

tvOS 13.0+

``` source
@MainActor
var customOverlayViewController: UIViewController? { get set }
```

## Discussion

The system presents the overlay view when the user swipes up on the Siri Remote during playback when the transport bar is hidden, or when they select a button when the transport bar is visible.

Important

Set a custom overlay view controller instead of installing a custom swipe gesture recognizer.

## See Also

### Customizing the tvOS Player UI

var playbackControlsIncludeTransportBar: Bool

A Boolean value that indicates whether the player shows the transport bar and related controls.

var playbackControlsIncludeInfoViews: Bool

A Boolean value that indicates whether the player presents video metadata, navigation markers, and playback settings views when the user requests them.

var transportBarIncludesTitleView: Bool

A Boolean value that indicates whether the player user interface shows the title view above the scrubber.

var transportBarCustomMenuItems: [UIMenuElement]

An array of actions and menus to display with the default player controls.

var customInfoViewControllers: [UIViewController]

An array of view controllers to display as content tabs in the player user interface.

var infoViewActions: [UIAction]!

An array of actions to present in the Info content view.

var contextualActions: [UIAction]

An array of action controls to present contextually during playback.

var unobscuredContentGuide: UILayoutGuide

A layout guide that represents an area that fixed-position playback controls don’t obscure when visible.

var customInfoViewController: UIViewController?

A view controller that provides client-specific content and controls alongside system-provided information and settings panels.

Deprecated

