

- Core Image
- CIImage
-  CIImageAutoAdjustmentOption 

Structure

# CIImageAutoAdjustmentOption

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
struct CIImageAutoAdjustmentOption
```

## Topics

### Initializers

init(rawValue: String)

### Type Properties

static let crop: CIImageAutoAdjustmentOption

A key used to specify whether to return a filter that crops the image to focus on detected features.

static let enhance: CIImageAutoAdjustmentOption

A key used to specify whether to return enhancement filters.

static let features: CIImageAutoAdjustmentOption

A key used to specify an array of features that you want to apply enhancement and red eye filters to.

static let level: CIImageAutoAdjustmentOption

A key used to specify whether to return a filter that rotates the image to keep a level perspective.

static let redEye: CIImageAutoAdjustmentOption

A key used to specify whether to return a red eye filter.

## Relationships

### Conforms To

- Hashable
- RawRepresentable
- Sendable

