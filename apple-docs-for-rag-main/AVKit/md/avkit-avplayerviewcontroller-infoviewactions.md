

- AVKit
- AVPlayerViewController
-  infoViewActions 

Instance Property

# infoViewActions

An array of actions to present in the Info content view.

tvOS 15.0+visionOS 1.0+

``` source
@MainActor
var infoViewActions: [UIAction]! { get set }
```

## Mentioned in 

Customizing the tvOS Playback Experience

Adopting the system player interface in visionOS

## Discussion

The Info content view can display up to two custom action controls along its trailing edge. The default value of this property is a single action that plays the current media from the beginning when tapped.

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

var contextualActions: [UIAction]

An array of action controls to present contextually during playback.

var customOverlayViewController: UIViewController?

A view controller that presents custom content over the player view.

var unobscuredContentGuide: UILayoutGuide

A layout guide that represents an area that fixed-position playback controls don’t obscure when visible.

var customInfoViewController: UIViewController?

A view controller that provides client-specific content and controls alongside system-provided information and settings panels.

Deprecated

