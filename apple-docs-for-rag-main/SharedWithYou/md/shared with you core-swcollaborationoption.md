

- Shared With You Core
-  SWCollaborationOption 

Class

# SWCollaborationOption

An object that determines how the system shares a document in a collaboration.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class SWCollaborationOption
```

## Overview

The `SWCollaborationOption` represents a user-configurable setting for a collaboration that the system uses to share the document. The system displays these options on the Share Sheet or in Messages.

## Topics

### Creating collaboration options

init(title: String, identifier: String)

Creates and initializes a collaboration option object with a provided title and identifier.

convenience init(title: String, identifier: String, subtitle: String, selected: Bool, requiredOptionsIdentifiers: [String])

Creates and initializes a collaboration option object with the provided values.

### Accessing option attributes

var identifier: String

A unique identifier.

var isSelected: Bool

A Boolean value that represents the selected state of an option.

var requiredOptionsIdentifiers: [String]

An array of option identifiers that the app must select before the system makes the option interactive.

var subtitle: String

A localized string the system displays to represent the permissions option in the collaboration view.

var title: String

A localized string the system displays as a title to represent the permissions option.

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

