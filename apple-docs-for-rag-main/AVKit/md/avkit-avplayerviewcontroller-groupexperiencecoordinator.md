

- AVKit
- AVPlayerViewController
-  groupExperienceCoordinator 

Instance Property

# groupExperienceCoordinator

The group experience coordinator for this view controller.

visionOS 2.0+

``` source
@MainActor
var groupExperienceCoordinator: AVGroupExperienceCoordinator { get }
```

## Discussion

Use this property to coordinate a group experience among participating view controllers.

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

var contextualActionsPreviewImage: UIImage?

An image to show alongside the contextual actions.

var requiresMonoscopicViewingMode: Bool

A Boolean value that indicates whether to permit playback of 2D video content only.

var experienceController: AVExperienceController

The experience controller for this view controller.

