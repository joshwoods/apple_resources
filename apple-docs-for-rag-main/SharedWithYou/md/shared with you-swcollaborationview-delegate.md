

- Shared With You
- SWCollaborationView
-  delegate 

Instance Property

# delegate

The delegate object for the collaboration view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any SWCollaborationViewDelegate)? { get set }
```

## See Also

### Accessing view attributes

var activeParticipantCount: Int

The number of participants in a collaboration.

var cloudSharingDelegate: (any UICloudSharingControllerDelegate)?

The delegate object for the cloud-sharing controller.

var headerImage: UIImage

The image that the system displays in the header.

var headerSubtitle: String

The subtitle that the system displays in the header.

var headerTitle: String

The title that the system displays in the header.

var manageButtonTitle: String

The manage button title that the system displays in the header.

var menuFormRepresentation: NSMenuItem

Returns a menu item suitable to display the collaboration detail view from the toolbar overflow menu.

var menuFormRepresentation: NSMenuItem

Returns a menu item suitable to display the collaboration detail view from the toolbar overflow menu.

