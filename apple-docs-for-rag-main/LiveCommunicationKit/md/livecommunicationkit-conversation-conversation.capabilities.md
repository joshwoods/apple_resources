

- LiveCommunicationKit
- Conversation
-  Conversation.Capabilities 

Structure

# Conversation.Capabilities

Used to configure a `Conversation` as part of a `Conversation.Update`.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
struct Capabilities
```

## Topics

### Initializers

init(rawValue: Int)

Creates a new option set from the given raw value.

### Instance Properties

var rawValue: Int

The corresponding value of the raw type.

### Type Aliases

typealias ArrayLiteralElement

The type of the elements of an array literal.

typealias Element

The element type of the option set.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static let merging: Conversation.Capabilities

The conversation can be merged with another conversation, creating a single conversation that is displayed to the user.

static let pausing: Conversation.Capabilities

The conversation can be temporarily paused including stopping all microphone, camera, and speaker interaction.

static let playingTones: Conversation.Capabilities

The conversation supports playing tone sequences.

static let unmerging: Conversation.Capabilities

Once merged, a conversation can be unmerged and reconfigured to act as a separate conversation.

static let video: Conversation.Capabilities

The conversation includes video streams to be displayed to or sent from the user.

### Default Implementations

Equatable Implementations

OptionSet Implementations

RawRepresentable Implementations

SetAlgebra Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- ExpressibleByArrayLiteral
- Hashable
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

