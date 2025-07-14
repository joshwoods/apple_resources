

- Audio Toolbox
-  CAFPacketTableHeader 

Structure

# CAFPacketTableHeader

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct CAFPacketTableHeader
```

## Topics

### Initializers

init()

init(mNumberPackets: Int64, mNumberValidFrames: Int64, mPrimingFrames: Int32, mRemainderFrames: Int32, mPacketDescriptions: UInt8)

### Instance Properties

var mNumberPackets: Int64

var mNumberValidFrames: Int64

var mPacketDescriptions: UInt8

var mPrimingFrames: Int32

var mRemainderFrames: Int32

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### File Structure

struct CAFAudioDescription

struct CAFAudioFormatListItem

struct CAFChunkHeader

struct CAFDataChunk

struct CAFFileHeader

struct CAFFormatFlags

struct CAFInfoStrings

struct CAFInstrumentChunk

struct CAFMarker

struct CAFMarkerChunk

struct CAFOverviewChunk

struct CAFOverviewSample

struct CAFPeakChunk

struct CAFPositionPeak

struct CAFRegion

