

- Shared With You
-  SWCollaborationView 

Class

# SWCollaborationView

A view that contains the collaboration content and options.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
@MainActor
class SWCollaborationView
```

## Mentioned in 

Adding shared content collaboration to your app

## Overview

The system presents an `SWCollaborationView` that displays participants and sharing options to a collaborator. For CloudKit and iCloud Drive adopters, the collaboration view includes a manage button. The button brings up the manage user interface, where collaborators can add and remove participants or change the share settings.

## Topics

### Creating a collaboration view

init(itemProvider: NSItemProvider)

Creates and initializes a collaboration view.

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

var menuFormRepresentation: NSMenuItem

Returns a menu item suitable to display the collaboration detail view from the toolbar overflow menu.

### Setting view attributes

func setContent(UIView)

Sets the content view.

func setDetailViewListContent&lt;ListContent>(ListContent)

Sets the detail view for the list content.

func setDetailViewListContent&lt;ListContent>(() -> ListContent)

Sets the detail view for the list content from view builder closures.

func setShowManageButton(Bool)

A Boolean value the system uses to show or hide the default manage-participants button in the collaboration popover.

### Dismissing the popover

func dismissPopover((() -> Void)?)

Dismisses the popover.

### Customizing the cloud-sharing behavior

var cloudSharingControllerDelegate: (any UICloudSharingControllerDelegate)?

A reference to an object that conforms to the CloudKit sharing controller delegate protocol.

var cloudSharingServiceDelegate: (any NSCloudSharingServiceDelegate)?

A reference to an object that conforms to the cloud-sharing service delegate protocol.

## Relationships

### Inherits From

- NSView
- UIView

### Conforms To

- CALayerDelegate
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSDraggingDestination
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- Sendable
- UIAccessibilityIdentification
- UIActivityItemsConfigurationProviding
- UIAppearance
- UIAppearanceContainer
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

