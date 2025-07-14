

- Shared With You Core
-  SWCollaborationMetadata 

Class

# SWCollaborationMetadata

A model object for conveying data during a collaboration.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class SWCollaborationMetadata
```

## Mentioned in 

Adding custom collaboration to your app

Adding shared content collaboration to your app

## Overview

Use `SWCollaborationMetadata` to share content without using iCloud. The system wraps the metadata object in an NSItemProvider object to implement a custom collaboration infrastructure.

If your app uses SwiftUI, `SWCollaborationMetadata` is compatible with the Transferable protocol and the ShareLink view.

## Topics

### Creating collaboration metadata

init(localIdentifier: SWLocalCollaborationIdentifier)

Creates and initializes a collaboration metadata object for the specified local identifier.

init(collaborationIdentifier: SWCollaborationIdentifier)

Creates and initializes a collaboration metadata object for the specified global identifier.

### Accessing metadata attributes

var collaborationIdentifier: SWCollaborationIdentifier

A globally unique identifier that the app hosting the collaboration provides.

var defaultShareOptions: SWCollaborationShareOptions?

The collaboration options that the content supports.

var initiatorHandle: String?

The handle of the person who initiates the collaboration.

var initiatorNameComponents: PersonNameComponents?

The name of the person who initiates the collaboration.

var localIdentifier: SWLocalCollaborationIdentifier

A locally unique identifier for the item the metadata represents.

var title: String?

The title of the content.

var userSelectedShareOptions: SWCollaborationShareOptions?

The selected collaboration options from the person who sends the invitation.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSItemProviderReading
- NSItemProviderWriting
- NSMutableCopying
- NSObjectProtocol
- NSSecureCoding
- Transferable

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

