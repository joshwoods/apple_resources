

- Shared With You Core
-  SWStartCollaborationAction 

Class

# SWStartCollaborationAction

An object that represents the first action sent to an app when the user shares a collaboration.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class SWStartCollaborationAction
```

## Mentioned in 

Adding custom collaboration to your app

## Overview

The action contains an updated SWCollaborationMetadata that include the user-selected share options. Fulfill this action with the universal link and a device-independent identifier for the collaboration.

## Topics

### Accessing action attributes

var collaborationMetadata: SWCollaborationMetadata

An object for that conveys data during a collaboration.

### Fulfilling an action

func fulfill(using: URL, collaborationIdentifier: SWCollaborationIdentifier)

Informs an app to set up the universal link and device independent identifier to provide to the system.

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

class SWUpdateCollaborationParticipantsAction

An action that contains the cryptographic identities the system uses to add to or remove from an existing collaboration.

let UTCollaborationOptionsTypeIdentifier: String

A string constant for the options type identifier.

