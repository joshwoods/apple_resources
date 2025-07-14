

- AVKit
- AVPlayerViewController
-  experienceController 

Instance Property

# experienceController

The experience controller for this view controller.

visionOS 2.0+

``` source
@MainActor @preconcurrency
var experienceController: AVExperienceController { get }
```

## Discussion

Use an experience controller to transition a player to different experiences and observe experience transitions.

The use of the experience controller is mutually exclusive with a view controller’s existing API for managing the experience. After accessing the `experienceController` property, those methods will log an error and have no effect. Attempting to access this property may fail if these mutually-exclusive properties and methods have been used.

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

var groupExperienceCoordinator: AVGroupExperienceCoordinator

The group experience coordinator for this view controller.

