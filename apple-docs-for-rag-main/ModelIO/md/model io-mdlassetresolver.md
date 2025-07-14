

- Model I/O
-  MDLAssetResolver 

Protocol

# MDLAssetResolver

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
protocol MDLAssetResolver : NSObjectProtocol
```

## Topics

### Instance Methods

func canResolveAssetNamed(String) -> Bool

**Required**

func resolveAssetNamed(String) -> URL

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- MDLBundleAssetResolver
- MDLPathAssetResolver
- MDLRelativeAssetResolver

