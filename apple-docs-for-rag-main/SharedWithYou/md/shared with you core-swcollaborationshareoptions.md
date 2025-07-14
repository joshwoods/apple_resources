

- Shared With You Core
-  SWCollaborationShareOptions 

Class

# SWCollaborationShareOptions

An object that represents the state of the collaboration options for the document.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class SWCollaborationShareOptions
```

## Mentioned in 

Adding custom collaboration to your app

## Topics

### Creating share options

init(coder: NSCoder)

Creates and initializes a collaboration share options object.

convenience init(optionsGroups: [SWCollaborationOptionsGroup])

Creates and initializes a collaboration share options object with the array of groups.

init(optionsGroups: [SWCollaborationOptionsGroup], summary: String)

Creates and initializes a collaboration share options object the array of groups and a summary string.

### Accessing options attributes

var optionsGroups: [SWCollaborationOptionsGroup]

An array of options group objects to customize how the system shares the collaboration.

var summary: String

A localized string to summarize the collaboration options.

## Relationships

### Inherits From

- NSObject

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

