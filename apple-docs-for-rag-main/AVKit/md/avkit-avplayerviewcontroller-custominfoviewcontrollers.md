

- AVKit
- AVPlayerViewController
-  customInfoViewControllers 

Instance Property

# customInfoViewControllers

An array of view controllers to display as content tabs in the player user interface.

tvOS 15.0+visionOS 1.0+

``` source
@MainActor
var customInfoViewControllers: [UIViewController] { get set }
```

## Mentioned in 

Adopting the system player interface in visionOS

Customizing the tvOS Playback Experience

## Discussion

The system uses a view controller’s title property value as the content tab title. Set this property value before adding it to the array so that the title renders correctly in the player’s user interface.

Similarly, set a preferredContentSize value on the custom view controllers, or define appropriate auto layout constraints on their views, so the system sizes them correctly in the player user interface.

Important

The view with the greatest height determines the height of all of the content views. Set the height of your content views consistently to simplify layout, or verify that your content renders as intended if the system resizes it.

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

