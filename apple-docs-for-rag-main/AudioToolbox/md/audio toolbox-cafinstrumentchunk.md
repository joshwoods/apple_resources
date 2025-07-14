

- Audio Toolbox
-  CAFInstrumentChunk 

Structure

# CAFInstrumentChunk

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct CAFInstrumentChunk
```

## Topics

### Initializers

init()

init(mBaseNote: Float32, mMIDILowNote: UInt8, mMIDIHighNote: UInt8, mMIDILowVelocity: UInt8, mMIDIHighVelocity: UInt8, mdBGain: Float32, mStartRegionID: UInt32, mSustainRegionID: UInt32, mReleaseRegionID: UInt32, mInstrumentID: UInt32)

### Instance Properties

var mBaseNote: Float32

var mInstrumentID: UInt32

var mMIDIHighNote: UInt8

var mMIDIHighVelocity: UInt8

var mMIDILowNote: UInt8

var mMIDILowVelocity: UInt8

var mReleaseRegionID: UInt32

var mStartRegionID: UInt32

var mSustainRegionID: UInt32

var mdBGain: Float32

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

struct CAFMarker

struct CAFMarkerChunk

struct CAFOverviewChunk

struct CAFOverviewSample

struct CAFPacketTableHeader

struct CAFPeakChunk

struct CAFPositionPeak

struct CAFRegion

