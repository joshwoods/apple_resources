

- Shared With You
-  SWCollaborationViewDelegate 

Protocol

# SWCollaborationViewDelegate

A delegate object that the system notifies about changes to the collaboration popover state.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
protocol SWCollaborationViewDelegate : NSObjectProtocol
```

## Topics

### Responding to popover activity

func collaborationViewShouldPresentPopover(SWCollaborationView) -> Bool

Asks the delegate whether the system can display the popover.

func collaborationViewDidDismissPopover(SWCollaborationView)

Notifies the delegate after the system dismisses the popover.

func collaborationViewWillPresentPopover(SWCollaborationView)

Notifies the delegate before the system presents the popover.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Collaboration management

class SWCollaborationCoordinator

An object that contains the shared collaboration coordinator.

class SWCollaborationOption

An object that determines how the system shares a document in a collaboration.

class SWCollaborationOptionsGroup

An object that represents a group of collaboration options that the system displays together.

class SWCollaborationOptionsPickerGroup

An object that represents a group of collaboration options that the system displays together with mutually exclusive options.

class SWCollaborationShareOptions

An object that represents the state of the collaboration options for the document.

let UTCollaborationOptionsTypeIdentifier: String

A string constant for the options type identifier.

