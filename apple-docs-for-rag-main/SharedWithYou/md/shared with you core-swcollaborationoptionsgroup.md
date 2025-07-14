

- Shared With You Core
-  SWCollaborationOptionsGroup 

Class

# SWCollaborationOptionsGroup

An object that represents a group of collaboration options that the system displays together.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class SWCollaborationOptionsGroup
```

## Mentioned in 

Adding custom collaboration to your app

## Topics

### Creating a collaboration options group

init(identifier: String, options: [SWCollaborationOption])

Creates and initializes a collaboration options group object.

### Accessing options group attributes

var footer: String

A localized string that provides additional information for the group of options.

var identifier: String

A unique identifier.

var options: [SWCollaborationOption]

An array of collaboration options the system displays as a group.

var title: String

A localized string the system displays as the title of the group section.

## Relationships

### Inherits From

- NSObject

### Inherited By

- SWCollaborationOptionsPickerGroup

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

