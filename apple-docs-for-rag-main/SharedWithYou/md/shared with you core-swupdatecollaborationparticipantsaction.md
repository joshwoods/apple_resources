

- Shared With You Core
-  SWUpdateCollaborationParticipantsAction 

Class

# SWUpdateCollaborationParticipantsAction

An action that contains the cryptographic identities the system uses to add to or remove from an existing collaboration.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class SWUpdateCollaborationParticipantsAction
```

## Mentioned in 

Adding custom collaboration to your app

## Overview

Look up the target collaboration using the provided SWCollaborationMetadata. Associate the added participants with the resource on your app’s servers, and remove any identities included in the removedIdentities property.

## Topics

### Accessing action attributes

var collaborationMetadata: SWCollaborationMetadata

An object for conveying data during a collaboration.

var addedIdentities: [SWPerson.Identity]

An array of added identities in a collaboration.

var removedIdentities: [SWPerson.Identity]

An array of removed identities in a collaboration.

## Relationships

### Inherits From

- SWAction

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Classes

class SWAction

An object that represents a collaboration action.

protocol SWCollaborationActionHandler

A delegate to handle incoming collaboration actions from a collaboration coordinator.

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

let UTCollaborationOptionsTypeIdentifier: String

A string constant for the options type identifier.

