

- AVKit
- AVPlayerViewController
-  requiresMonoscopicViewingMode 

Instance Property

# requiresMonoscopicViewingMode

A Boolean value that indicates whether to permit playback of 2D video content only.

visionOS 1.0+

``` source
@MainActor
var requiresMonoscopicViewingMode: Bool { get set }
```

## Discussion

The default value is false.

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

var experienceController: AVExperienceController

The experience controller for this view controller.

var groupExperienceCoordinator: AVGroupExperienceCoordinator

The group experience coordinator for this view controller.

