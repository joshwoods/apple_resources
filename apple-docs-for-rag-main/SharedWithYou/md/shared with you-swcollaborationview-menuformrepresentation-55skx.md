

- Shared With You
- SWCollaborationView
-  menuFormRepresentation 

Instance Property

# menuFormRepresentation

Returns a menu item suitable to display the collaboration detail view from the toolbar overflow menu.

macOS 13.1+

``` source
@MainActor
var menuFormRepresentation: NSMenuItem { get }
```

## Discussion

If this SWCollaborationView instance is being set on an NSToolbarItem, assign this property to the item’s `menuFormRepresentation` property.

## See Also

### Accessing view attributes

var activeParticipantCount: Int

The number of participants in a collaboration.

var cloudSharingDelegate: (any UICloudSharingControllerDelegate)?

The delegate object for the cloud-sharing controller.

var delegate: (any SWCollaborationViewDelegate)?

The delegate object for the collaboration view.

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

