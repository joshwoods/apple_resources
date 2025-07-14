

- Shared With You
-  Collaboration views 

API Collection

# Collaboration views

Create and customize a collaboration view to manage the shared content actions.

## Topics

### Collaboration views

class SWCollaborationView

A view that contains the collaboration content and options.

### Collaboration attributes

class SWCollaborationHighlight

A highlight object that represents an active collaboration.

class SWCollaborationMetadata

A model object for conveying data during a collaboration.

struct SWCollaborationIdentifier

A unique identifier for a collaboration.

struct SWLocalCollaborationIdentifier

A local identifier for a collaboration.

let SWCollaborationMetadataTypeIdentifier: String

A string constant for the metadata type identifier.

### Collaboration management

protocol SWCollaborationViewDelegate

A delegate object that the system notifies about changes to the collaboration popover state.

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

### Actions

class SWAction

An object that represents a collaboration action.

class SWStartCollaborationAction

An object that represents the first action sent to an app when the user shares a collaboration.

protocol SWCollaborationActionHandler

A delegate to handle incoming collaboration actions from a collaboration coordinator.

class SWUpdateCollaborationParticipantsAction

An action that contains the cryptographic identities the system uses to add to or remove from an existing collaboration.

## See Also

### Collaboration

Adding shared content collaboration to your app

Manage shared content collaboration in your app using CloudKit and iCloud Drive.

Adding custom collaboration to your app

Integrate your custom collaboration app with Messages.

