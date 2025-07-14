

- Shared With You Core
-  SWCollaborationIdentifier 

Structure

# SWCollaborationIdentifier

A unique identifier for a collaboration.

``` source
struct SWCollaborationIdentifier
```

## Topics

### Creating a collaboration identifier

init(String)

Creates and initializes a collaboration identifier object.

init(rawValue: String)

Creates and initializes a collaboration identifier object.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Classes

class SWAction

An object that represents a collaboration action.

protocol SWCollaborationActionHandler

A delegate to handle incoming collaboration actions from a collaboration coordinator.

class SWCollaborationCoordinator

An object that contains the shared collaboration coordinator.

class SWCollaborationMetadata

A model object for conveying data during a collaboration.

class SWCollaborationOption

An object that determines how the system shares a document in a collaboration.

class SWCollaborationOptionsGroup

An object that represents a group of collaboration options that the system displays together.

class SWCollaborationOptionsPickerGroup

An object that represents a group of collaboration options that the system displays together with mutually exclusive options.

class SWCollaborationShareOptions

An object that represents the state of the collaboration options for the document.

struct SWLocalCollaborationIdentifier

A local identifier for a collaboration.

class SWPerson

An object that tracks participants in a collaboration.

class SWStartCollaborationAction

An object that represents the first action sent to an app when the user shares a collaboration.

class SWUpdateCollaborationParticipantsAction

An action that contains the cryptographic identities the system uses to add to or remove from an existing collaboration.

let UTCollaborationOptionsTypeIdentifier: String

A string constant for the options type identifier.

