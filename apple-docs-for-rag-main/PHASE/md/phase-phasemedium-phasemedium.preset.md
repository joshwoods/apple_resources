

- PHASE
- PHASEMedium
-  PHASEMedium.Preset 

Enumeration

# PHASEMedium.Preset

Predetermined qualities of an environment that affect how sound transmits.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
enum Preset
```

## Overview

Currently, this enumeration refers only to sound traveling through air.

## Topics

### Medium Types

case air

A medium that simulates sound traveling through air.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating a Medium

init(engine: PHASEEngine, preset: PHASEMedium.Preset)

Creates a medium.

