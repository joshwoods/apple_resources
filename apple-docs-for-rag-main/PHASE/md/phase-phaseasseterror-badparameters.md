

- PHASE
- PHASEAssetError
-  badParameters 

Type Property

# badParameters

An error that indicates an asset registry call contains invalid data.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
static var badParameters: PHASEAssetError.Code { get }
```

## See Also

### Identifying an Error Cause

static var alreadyExists: PHASEAssetError.Code

An error the asset registry throws when the app registers an asset twice by the same name.

static var failedToLoad: PHASEAssetError.Code

An error that indicates an asset failed to load.

static var generalError: PHASEAssetError.Code

An error the asset registry throws when an unspecified problem occurs.

static var invalidEngineInstance: PHASEAssetError.Code

An error that indicates an asset registry call references an invalid engine.

static var memoryAllocation: PHASEAssetError.Code

An error the framework throws when an asset depletes system memory.

