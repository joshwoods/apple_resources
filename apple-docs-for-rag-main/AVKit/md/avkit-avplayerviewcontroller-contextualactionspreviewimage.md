

- AVKit
- AVPlayerViewController
-  contextualActionsPreviewImage 

Instance Property

# contextualActionsPreviewImage

An image to show alongside the contextual actions.

visionOS 1.0+

``` source
@NSCopying @MainActor
var contextualActionsPreviewImage: UIImage? { get set }
```

## Discussion

Use this to enhance a contextual action with more context. For example, if the action presents a button to jump back in time, show a preview frame of where in the movie the action skips to.

Note

The system only displays an image if the contextualActions property contains a single value.

## See Also

### Configuring the visionOS Player UI

var infoViewActions: [UIAction]!

An array of actions to present in the Info content view.

var customInfoViewControllers: [UIViewController]

An array of view controllers to display as content tabs in the player user interface.

var contextualActions: [UIAction]

An array of action controls to present contextually during playback.

var contextualActionsInfoView: UIView

A view the system shows adjacent to the contextual actions that’s suitable for showing related information.

var requiresMonoscopicViewingMode: Bool

A Boolean value that indicates whether to permit playback of 2D video content only.

var experienceController: AVExperienceController

The experience controller for this view controller.

var groupExperienceCoordinator: AVGroupExperienceCoordinator

The group experience coordinator for this view controller.

