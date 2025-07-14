

- Shared With You Core
-  SWCollaborationActionHandler 

Protocol

# SWCollaborationActionHandler

A delegate to handle incoming collaboration actions from a collaboration coordinator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
protocol SWCollaborationActionHandler : NSObjectProtocol
```

## Mentioned in 

Adding custom collaboration to your app

## Topics

### Handling collaboration actions

func collaborationCoordinator(SWCollaborationCoordinator, handle: SWStartCollaborationAction)

Notifies the delegate when the system starts a collaboration.

**Required**

func collaborationCoordinator(SWCollaborationCoordinator, handle: SWUpdateCollaborationParticipantsAction)

Notifies the delegate when the system updates the participants in a collaboration.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Classes

class SWAction

An object that represents a collaboration action.

class SWCollaborationCoordinator

An object that contains the shared collaboration coordinator.

struct SWCollaborationIdentifier

A unique identifier for a collaboration.

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

