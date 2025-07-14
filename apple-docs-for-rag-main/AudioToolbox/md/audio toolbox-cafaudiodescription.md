

- Audio Toolbox
-  CAFAudioDescription 

Structure

# CAFAudioDescription

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct CAFAudioDescription
```

## Topics

### Initializers

init()

init(mSampleRate: Float64, mFormatID: UInt32, mFormatFlags: CAFFormatFlags, mBytesPerPacket: UInt32, mFramesPerPacket: UInt32, mChannelsPerFrame: UInt32, mBitsPerChannel: UInt32)

### Instance Properties

var mBitsPerChannel: UInt32

var mBytesPerPacket: UInt32

var mChannelsPerFrame: UInt32

var mFormatFlags: CAFFormatFlags

var mFormatID: UInt32

var mFramesPerPacket: UInt32

var mSampleRate: Float64

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### File Structure

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

struct CAFPacketTableHeader

struct CAFPeakChunk

struct CAFPositionPeak

struct CAFRegion

