

- Core Media
-  CMSampleBuffer 

Class

# CMSampleBuffer

A reference to a buffer of media data.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
class CMSampleBuffer
```

## Overview

A sample buffer is a Core Foundation object that contains zero or more media samples of a particular type (audio, video, muxed, and so on).

## Topics

### Determining Readiness

var dataReadiness: CMSampleBuffer.DataReadiness

A value that indicates the status of the data the sample buffer contains.

func setDataReadiness(CMSampleBuffer.DataReadiness) throws

Sets the status of the sample buffer’s data.

enum DataReadiness

Constants that indicate the readiness of a sample buffer’s data.

func makeDataReady() throws

Makes the sample buffer’s data ready for use by calling its handler closure.

func trackDataReadiness(CMSampleBuffer) throws

Associates a sample buffer’s data readiness with that of another sample buffer.

### Invalidating Sample Buffers

var isValid: Bool

A Boolean value that indicates whether the sample buffer is valid.

func setInvalidateHandler((CMSampleBuffer) throws -> Void) throws

Sets a closure for the sample buffer to call when it’s invalidated.

func invalidate() throws

Invalidates a sample buffer by calling its invalidation handler.

### Inspecting Size Information

var numSamples: Int

The number of media samples the buffer contains.

func sampleSizes() throws -> [Int]

Retrieves an array of sample sizes that represents each sample in a sample buffer.

func sampleSize(at: Int) -> Int

Returns the size of a sample in bytes.

var totalSampleSize: Int

The total size in bytes of sample data in the buffer.

### Inspecting Duration and Timing

var duration: CMTime

The total duration of a sample buffer.

var decodeTimeStamp: CMTime

The decode timestamp of the first sample in the buffer.

var presentationTimeStamp: CMTime

The sample presentation timestamp that’s the earliest numerically in the sample buffer.

var outputDuration: CMTime

The output duration of the sample buffer.

var outputDecodeTimeStamp: CMTime

The output decode timestamp for a sample buffer.

var outputPresentationTimeStamp: CMTime

The output presentation timestamp of a sample buffer.

func setOutputPresentationTimeStamp(CMTime) throws

Sets an output presentation timestamp to use in place of a calculated value.

func sampleTimingInfos() throws -> [CMSampleTimingInfo]

Retrieves an array of sample timing information structures that represents each sample in a sample buffer.

func sampleTimingInfo(at: CMItemIndex) throws -> CMSampleTimingInfo

Returns sample timing information for a sample at the specified index.

func outputSampleTimingInfos() throws -> [CMSampleTimingInfo]

Retrieves an array of output sample timing information structures that represents each sample in a sample buffer.

### Accessing the Format Description

var formatDescription: CMFormatDescription?

An object that describes the details of the media data.

### Modifying Sample Buffers

var dataBuffer: CMBlockBuffer?

A block buffer that contains the media data.

func setDataBuffer(CMBlockBuffer) throws

Associates a block buffer of media data with a sample buffer.

var imageBuffer: CVImageBuffer?

An image buffer that contains the media data.

func withAudioBufferList&lt;R>(blockBufferMemoryAllocator: CFAllocator?, flags: CMSampleBuffer.Flags, body: (UnsafeMutableAudioBufferListPointer, CMBlockBuffer) throws -> R) throws -> R

Calls a closure with an audio buffer list that contains the data from a sample buffer and a block buffer backing the audio buffers.

func setDataBuffer(fromAudioBufferList: UnsafePointer&lt;AudioBufferList>, blockBufferMemoryAllocator: CFAllocator?, flags: CMSampleBuffer.Flags) throws

Creates a block buffer that contains a copy of the data from an audio buffer list, and sets it as the sample buffer’s data.

func copyPCMData(fromRange: Range&lt;Int>, into: UnsafeMutablePointer&lt;AudioBufferList>) throws

Copies PCM audio data from a sample buffer into a prepopulated audio buffer list.

func audioStreamPacketDescriptions() throws -> [AudioStreamPacketDescription]

Creates an array of audio stream packet descriptions for the variable bytes per packet or variable frames per packet audio data in a sample buffer.

func withUnsafeAudioStreamPacketDescriptions&lt;R>((UnsafeBufferPointer&lt;AudioStreamPacketDescription>) throws -> R) throws -> R

Calls a closure with an audio stream packet description.

func singleSampleBuffers() throws -> CMSampleBuffer.SingleSampleBuffers

Returns all samples in a sample buffer.

struct SingleSampleBuffers

A structure that holds all samples in a sample buffer.

### Managing Attachments

struct AttachmentKey

Keys that identify sample buffer attachments.

var sampleAttachments: CMSampleBuffer.SampleAttachmentsArray

An array of sample attachments.

struct SampleAttachmentsArray

A structure that defines an array of sample attachments.

struct PerSampleAttachmentsDictionary

A structure that defines keys to identify per-sample attachments.

### Accessing the Type Identifier

static var typeID: CFTypeID

Returns the type identifier of sample buffer objects.

### Accessing Tagged Buffers

var taggedBuffers: [CMTaggedBuffer]?

Returns the tagged buffers associated with this buffer.

### Constants

struct Error

A structure that defines errors that occur during framework operations.

struct Flags

Flags that customize the behavior of framework operations.

struct NotificationKey

A key for sample buffer notifications.

### Notifications

static let dataBecameReady: NSNotification.Name

A notification the system posts when a sample buffer’s data becomes ready.

static let dataFailed: NSNotification.Name

A notification the system posts when a sample buffer fails to load its data.

## Relationships

### Conforms To

- CMAttachmentBearerProtocol
- Copyable
- Equatable
- Hashable

## See Also

### Data Types

Sample Buffer Flags

Flags that customize the behavior of framework operations.

struct CMSampleTimingInfo

A collection of timing information for a sample in a sample buffer.

typealias CMBuffer

A reference to a buffer object.

typealias CMBufferGetSizeCallback

A client callback that returns a size.

typealias CMItemIndex

A datatype that represents an item index.

typealias CMItemCount

A datatype that represents an item count.

typealias CMPersistentTrackID

A datatype that represents a persistent track identifier.

typealias CMMuxedStreamType

A datatype that represents a muxed stream of data.

