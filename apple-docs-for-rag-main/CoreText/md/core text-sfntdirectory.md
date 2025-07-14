

- Core Text
-  sfntDirectory 

Structure

# sfntDirectory

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct sfntDirectory
```

## Topics

### Initializers

init()

init(format: FourCharCode, numOffsets: UInt16, searchRange: UInt16, entrySelector: UInt16, rangeShift: UInt16, table: sfntDirectoryEntry)

### Instance Properties

var entrySelector: UInt16

var format: FourCharCode

var numOffsets: UInt16

var rangeShift: UInt16

var searchRange: UInt16

var table: sfntDirectoryEntry

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

