

- PHASE
- PHASEAssetError
-  PHASEAssetError.Code 

Enumeration

# PHASEAssetError.Code

Codes that identify framework asset errors.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
enum Code
```

## Topics

### Errors

case alreadyExists

An error the asset registry throws when the app registers an asset twice by the same name.

case badParameters

An error that indicates an asset registry call contains invalid data.

case failedToLoad

An error that indicates an asset failed to load.

case generalError

An error the asset registry throws when an unspecified problem occurs.

case invalidEngineInstance

An error that indicates an asset registry call references an invalid engine.

case memoryAllocation

An error the framework throws when an asset depletes system memory.

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

### Asset Errors

struct PHASEAssetError

An asset error that PHASE reports.

let PHASEAssetErrorDomain: String

A unique error domain for PHASE assets.

