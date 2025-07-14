

- PHASE
- PHASEAsset
-  PHASEAsset.AssetType 

Enumeration

# PHASEAsset.AssetType

Options that determine how PHASE manages sound assets in memory.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
enum AssetType
```

## Overview

To prepare for playback, the framework can decompress a sound asset or perform a format conversion, or both, depending on the type of the underlying asset data.

## Topics

### Types

case resident

A sound asset that plays after fully loading in memory.

case streamed

A sound asset that streams from disk into memory as it plays.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

