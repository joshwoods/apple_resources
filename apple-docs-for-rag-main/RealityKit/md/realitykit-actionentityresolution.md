

- RealityKit
-  ActionEntityResolution 

Enumeration

# ActionEntityResolution

Options available to determine the resolution method for a target entity in an action.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
enum ActionEntityResolution
```

## Overview

Use this to resolve the entity an action should target. For example, ImpulseAction structure accepts this enumeration as an initializer argument to resolve the entity.

## Topics

### Operators

static func == (ActionEntityResolution, ActionEntityResolution) -> Bool

Indicates whether two action entity resolutions are equal.

### Enumeration Cases

case entityNamed(String)

An option that resolves an entity from the specified name within the scene of the entity playing the action.

case entityPath(BindTarget.EntityPath)

An option that resolves an entity by specifying a bind path relative to the entity playing the action.

### Initializers

init(from: any Decoder) throws

Creates a new instance from a decoder.

### Instance Methods

func encode(to: any Encoder) throws

Writes the action entity resolution data into an encoder.

### Type Properties

static var sourceEntity: ActionEntityResolution

Resolves to the source entity that is playing the action.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable

## See Also

### Action management

protocol EntityAction

A protocol that defines an action for an entity.

struct ActionAnimation

Defines an an action animation.

protocol ActionHandlerProtocol

The base protocol for action handlers.

