

- Core Text
-  sfntVariationHeader 

Structure

# sfntVariationHeader

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct sfntVariationHeader
```

## Topics

### Initializers

init()

init(version: Fixed, offsetToData: UInt16, countSizePairs: UInt16, axisCount: UInt16, axisSize: UInt16, instanceCount: UInt16, instanceSize: UInt16, axis: sfntVariationAxis, instance: sfntInstance)

### Instance Properties

var axis: sfntVariationAxis

var axisCount: UInt16

var axisSize: UInt16

var countSizePairs: UInt16

var instance: sfntInstance

var instanceCount: UInt16

var instanceSize: UInt16

var offsetToData: UInt16

var version: Fixed

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

