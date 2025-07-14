

- Core Text
-  sfntFeatureHeader 

Structure

# sfntFeatureHeader

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct sfntFeatureHeader
```

## Topics

### Initializers

init()

init(version: Int32, featureNameCount: UInt16, featureSetCount: UInt16, reserved: Int32, names: sfntFeatureName, settings: sfntFontFeatureSetting, runs: sfntFontRunFeature)

### Instance Properties

var featureNameCount: UInt16

var featureSetCount: UInt16

var names: sfntFeatureName

var reserved: Int32

var runs: sfntFontRunFeature

var settings: sfntFontFeatureSetting

var version: Int32

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Structures

struct AnchorPoint

struct AnchorPointTable

struct AnkrTable

struct BslnFormat0Part

struct BslnFormat1Part

struct BslnFormat2Part

struct BslnFormat3Part

struct BslnFormatUnion

struct BslnTable

struct FontVariation

struct JustDirectionTable

struct JustPCAction

struct JustPCActionSubrecord

struct JustPCConditionalAddAction

struct JustPCDecompositionAction

