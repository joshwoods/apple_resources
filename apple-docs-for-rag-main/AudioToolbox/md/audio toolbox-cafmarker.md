

- Audio Toolbox
-  CAFMarker 

Structure

# CAFMarker

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct CAFMarker
```

## Topics

### Initializers

init()

init(mType: UInt32, mFramePosition: Float64, mMarkerID: UInt32, mSMPTETime: CAF_SMPTE_Time, mChannel: UInt32)

### Instance Properties

var mChannel: UInt32

var mFramePosition: Float64

var mMarkerID: UInt32

var mSMPTETime: CAF_SMPTE_Time

var mType: UInt32

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

struct CAFMarkerChunk

struct CAFOverviewChunk

struct CAFOverviewSample

struct CAFPacketTableHeader

struct CAFPeakChunk

struct CAFPositionPeak

struct CAFRegion

