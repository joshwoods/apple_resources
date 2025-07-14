

- AVKit
- AVPlayerViewController
-  contextualActions 

Instance Property

# contextualActions

An array of action controls to present contextually during playback.

tvOS 15.0+visionOS 1.0+

``` source
@MainActor
var contextualActions: [UIAction] { get set }
```

## Mentioned in 

Customizing the tvOS Playback Experience

Adopting the system player interface in visionOS

## Discussion

Use this property to present action controls for a specific time in the presentation, such as showing a Skip Intro button during a title sequence. Have your app observe the player’s timing, and when playback reaches a point at which to present controls, set the property value to one or more custom actions. To dismiss the controls, set this property value back to an empty array.

For details about observing player timing, see `Observing the Playback Time`.

Note

The view controller presents contextual actions only when the transport bar isn’t visible.

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

var customOverlayViewController: UIViewController?

A view controller that presents custom content over the player view.

var unobscuredContentGuide: UILayoutGuide

A layout guide that represents an area that fixed-position playback controls don’t obscure when visible.

var customInfoViewController: UIViewController?

A view controller that provides client-specific content and controls alongside system-provided information and settings panels.

Deprecated

