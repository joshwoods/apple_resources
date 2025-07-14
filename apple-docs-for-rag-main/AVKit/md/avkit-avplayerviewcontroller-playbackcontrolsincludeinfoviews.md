

- AVKit
- AVPlayerViewController
-  playbackControlsIncludeInfoViews 

Instance Property

# playbackControlsIncludeInfoViews

A Boolean value that indicates whether the player presents video metadata, navigation markers, and playback settings views when the user requests them.

tvOS 11.0+

``` source
@MainActor
var playbackControlsIncludeInfoViews: Bool { get set }
```

## Discussion

This property determines whether the player shows views for video metadata, navigation markers, and playback settings. Set this property value to false, and showsPlaybackControls to true, to selectively prevent the player from displaying its information and setting panels. Changing the value of this property doesn’t immediately change the visibility of the info views.

The default value is true.

## See Also

### Customizing the tvOS Player UI

var playbackControlsIncludeTransportBar: Bool

A Boolean value that indicates whether the player shows the transport bar and related controls.

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

var customOverlayViewController: UIViewController?

A view controller that presents custom content over the player view.

var unobscuredContentGuide: UILayoutGuide

A layout guide that represents an area that fixed-position playback controls don’t obscure when visible.

var customInfoViewController: UIViewController?

A view controller that provides client-specific content and controls alongside system-provided information and settings panels.

Deprecated

