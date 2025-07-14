

- RealityKit
- FromToByAction
-  FromToByAction.TransformMode 

Enumeration

# FromToByAction.TransformMode

Options available to determine the space the bound entity should be relative to.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
enum TransformMode
```

## Overview

The FromToByAction structure accepts this enumeration as an initializer argument when the FromToByAction value is a Transform type.

## Topics

### Operators

static func == (FromToByAction&lt;Value>.TransformMode, FromToByAction&lt;Value>.TransformMode) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case local

The provided transforms are relative to the transform of the bound entity.

case parent

The provided transforms are relative to the bound entities parent transform.

case relative(to: ActionEntityResolution)

The provided transforms are relative to the resolved entities transform.

case scene

The provided transform is relative to the scene, in world space.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

### Type Properties

static var `default`: FromToByAction&lt;Value>.TransformMode

Default transform mode used by the specializations which use transform mode.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable

