

- Shared With You Core
-  SWCollaborationCoordinator 

Class

# SWCollaborationCoordinator

An object that contains the shared collaboration coordinator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class SWCollaborationCoordinator
```

## Overview

`SWCollaborationCoordinator` is a singleton, meaning there’s a global shared instance. The singleton invokes its actionHandler delegate to coordinate new collaborations and updates to existing collaborations.

Register the delegate soon after launch and handle actions immediately to avoid timeouts. Here’s how to set up the collaboration coordinator after your app finishes launching:

1.  Access the singleton coordinator instance through the shared property.

2.  Then, in the app delegate’s application(_:didFinishLaunchingWithOptions:) method, set the `actionHandler` property to an object that conforms to the SWCollaborationActionHandler protocol.

Related Sessions from WWDC22

Session 10093: Integrate your custom collaboration app with Messages

## Topics

### Accessing coordinator attributes

class var shared: SWCollaborationCoordinator

The shared collaboration coordinator.

var actionHandler: (any SWCollaborationActionHandler)?

The collaboration action handler.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Classes

class SWAction

An object that represents a collaboration action.

protocol SWCollaborationActionHandler

A delegate to handle incoming collaboration actions from a collaboration coordinator.

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

