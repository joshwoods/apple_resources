

- Core Media
-  CMSampleBuffer APIs 

API Collection

# CMSampleBuffer APIs

An object that contains zero or more media samples of a uniform media type.

## Overview

Sample buffers are Core Foundation objects that the system uses to move media sample data through the media pipeline. An instance of `CMSampleBuffer` contains zero or more compressed (or uncompressed) samples of a particular media type and contains one of the following:

- A CMBlockBuffer of one or more media samples

- A CVImageBuffer, a reference to the format description for the stream of `CMSampleBuffers`, size and timing information for each of the contained media samples, and both buffer-level and sample-level attachments

A sample buffer can contain both sample-level and buffer-level attachments. Each individual sample in a buffer may provide attachments that include information such as timestamps and video frame dependencies. You read and write sample-level attachments using the CMSampleBufferGetSampleAttachmentsArray(_:createIfNecessary:) function. Buffer-level attachments provide information about the buffer as a whole, such as playback speed and actions to perform upon consuming the buffer. You can read and write buffer-level attachments using the APIs described in CMAttachment APIs and the keys listed under Sample Attachment Keys.

It’s possible for a sample buffer to describe samples it doesn’t yet contain. For example, some media services may have access to sample size, timing, and format information before they read the data. Such services may create sample buffers with that information and insert them into queues early, and attach (or fill) the buffer of media data later, when it becomes ready. Sample buffers have the concept of data-readiness, which means you can test, set, and force them to become ready “now.” It’s also possible for a sample buffer to contain nothing but a special buffer-level attachment that describes a media stream event (for example, “discontinuity: drain and reset decoder before processing the next `CMSampleBuffer`”).

## Topics

### Creating Sample Buffers

func CMSampleBufferCreateReady(allocator: CFAllocator?, dataBuffer: CMBlockBuffer?, formatDescription: CMFormatDescription?, sampleCount: CMItemCount, sampleTimingEntryCount: CMItemCount, sampleTimingArray: UnsafePointer&lt;CMSampleTimingInfo>?, sampleSizeEntryCount: CMItemCount, sampleSizeArray: UnsafePointer&lt;Int>?, sampleBufferOut: UnsafeMutablePointer&lt;CMSampleBuffer?>) -> OSStatus

Creates a sample buffer with media data.

func CMSampleBufferCreateReadyWithImageBuffer(allocator: CFAllocator?, imageBuffer: CVImageBuffer, formatDescription: CMVideoFormatDescription, sampleTiming: UnsafePointer&lt;CMSampleTimingInfo>, sampleBufferOut: UnsafeMutablePointer&lt;CMSampleBuffer?>) -> OSStatus

Creates a sample buffer with image data.

func CMAudioSampleBufferCreateReadyWithPacketDescriptions(allocator: CFAllocator?, dataBuffer: CMBlockBuffer, formatDescription: CMFormatDescription, sampleCount: CMItemCount, presentationTimeStamp: CMTime, packetDescriptions: UnsafePointer&lt;AudioStreamPacketDescription>?, sampleBufferOut: UnsafeMutablePointer&lt;CMSampleBuffer?>) -> OSStatus

Creates a sample buffer with packet descriptions.

func CMSampleBufferCreateWithMakeDataReadyHandler(CFAllocator?, CMBlockBuffer?, Bool, CMFormatDescription?, CMItemCount, CMItemCount, UnsafePointer&lt;CMSampleTimingInfo>?, CMItemCount, UnsafePointer&lt;Int>?, UnsafeMutablePointer&lt;CMSampleBuffer?>, CMSampleBufferMakeDataReadyHandler?) -> OSStatus

Creates a sample buffer with a handler to make the data ready for use.

func CMSampleBufferCreateForImageBufferWithMakeDataReadyHandler(CFAllocator?, CVImageBuffer, Bool, CMVideoFormatDescription, UnsafePointer&lt;CMSampleTimingInfo>, UnsafeMutablePointer&lt;CMSampleBuffer?>, CMSampleBufferMakeDataReadyHandler?) -> OSStatus

Creates a sample buffer with an image buffer and a handler to make the data ready for use.

func CMAudioSampleBufferCreateWithPacketDescriptionsAndMakeDataReadyHandler(CFAllocator?, CMBlockBuffer?, Bool, CMFormatDescription, CMItemCount, CMTime, UnsafePointer&lt;AudioStreamPacketDescription>?, UnsafeMutablePointer&lt;CMSampleBuffer?>, CMSampleBufferMakeDataReadyHandler?) -> OSStatus

Creates a sample buffer with packet descriptions and a handler to make the data ready for use.

func CMSampleBufferCreate(allocator: CFAllocator?, dataBuffer: CMBlockBuffer?, dataReady: Bool, makeDataReadyCallback: CMSampleBufferMakeDataReadyCallback?, refcon: UnsafeMutableRawPointer?, formatDescription: CMFormatDescription?, sampleCount: CMItemCount, sampleTimingEntryCount: CMItemCount, sampleTimingArray: UnsafePointer&lt;CMSampleTimingInfo>?, sampleSizeEntryCount: CMItemCount, sampleSizeArray: UnsafePointer&lt;Int>?, sampleBufferOut: UnsafeMutablePointer&lt;CMSampleBuffer?>) -> OSStatus

Creates a sample buffer with a callback to make the data ready for use.

func CMSampleBufferCreateForImageBuffer(allocator: CFAllocator?, imageBuffer: CVImageBuffer, dataReady: Bool, makeDataReadyCallback: CMSampleBufferMakeDataReadyCallback?, refcon: UnsafeMutableRawPointer?, formatDescription: CMVideoFormatDescription, sampleTiming: UnsafePointer&lt;CMSampleTimingInfo>, sampleBufferOut: UnsafeMutablePointer&lt;CMSampleBuffer?>) -> OSStatus

Creates a sample buffer with an image buffer and a callback to make the data ready for use.

func CMAudioSampleBufferCreateWithPacketDescriptions(allocator: CFAllocator?, dataBuffer: CMBlockBuffer?, dataReady: Bool, makeDataReadyCallback: CMSampleBufferMakeDataReadyCallback?, refcon: UnsafeMutableRawPointer?, formatDescription: CMFormatDescription, sampleCount: CMItemCount, presentationTimeStamp: CMTime, packetDescriptions: UnsafePointer&lt;AudioStreamPacketDescription>?, sampleBufferOut: UnsafeMutablePointer&lt;CMSampleBuffer?>) -> OSStatus

Creates a sample buffer with packet descriptions and a callback to make the data ready for use.

### Copying Sample Buffers

func CMSampleBufferCreateCopy(allocator: CFAllocator?, sampleBuffer: CMSampleBuffer, sampleBufferOut: UnsafeMutablePointer&lt;CMSampleBuffer?>) -> OSStatus

Creates a copy of a sample buffer.

func CMSampleBufferCreateCopyWithNewTiming(allocator: CFAllocator?, sampleBuffer: CMSampleBuffer, sampleTimingEntryCount: CMItemCount, sampleTimingArray: UnsafePointer&lt;CMSampleTimingInfo>?, sampleBufferOut: UnsafeMutablePointer&lt;CMSampleBuffer?>) -> OSStatus

Creates a copy of a sample buffer with new timing information.

func CMSampleBufferCopySampleBufferForRange(allocator: CFAllocator?, sampleBuffer: CMSampleBuffer, sampleRange: CFRange, sampleBufferOut: UnsafeMutablePointer&lt;CMSampleBuffer?>) -> OSStatus

Creates a sample buffer that contains a range of samples from an existing sample buffer.

### Determining Readiness

func CMSampleBufferDataIsReady(CMSampleBuffer) -> Bool

Returns a Boolean value that indicates whether the sample buffer’s data is ready for use.

func CMSampleBufferSetDataReady(CMSampleBuffer) -> OSStatus

Marks a sample buffer’s data as ready for use.

func CMSampleBufferSetDataFailed(CMSampleBuffer, status: OSStatus) -> OSStatus

Marks the sample buffer’s data as failed to indicate that it won’t become ready.

func CMSampleBufferHasDataFailed(CMSampleBuffer, statusOut: UnsafeMutablePointer&lt;OSStatus>?) -> Bool

Returns a Boolean value that indicates whether the sample buffer’s data loading request failed.

func CMSampleBufferMakeDataReady(CMSampleBuffer) -> OSStatus

Makes the sample buffer’s data ready for use by invoking its callback to load the data.

func CMSampleBufferTrackDataReadiness(CMSampleBuffer, sampleBufferToTrack: CMSampleBuffer) -> OSStatus

Associates a sample buffer’s data readiness with that of another sample buffer.

### Invalidating Sample Buffers

func CMSampleBufferSetInvalidateHandler(CMSampleBuffer, invalidateHandler: CMSampleBufferInvalidateHandler) -> OSStatus

Sets the sample buffer’s invalidation handler.

func CMSampleBufferInvalidate(CMSampleBuffer) -> OSStatus

Invalidates a sample buffer by calling its invalidation callback.

func CMSampleBufferIsValid(CMSampleBuffer) -> Bool

Returns a Boolean value that indicates whether a sample buffer is valid.

func CMSampleBufferSetInvalidateCallback(CMSampleBuffer, callback: CMSampleBufferInvalidateCallback, refcon: UInt64) -> OSStatus

Sets the sample buffer’s invalidation callback.

### Inspecting Size Information

func CMSampleBufferGetNumSamples(CMSampleBuffer) -> CMItemCount

Returns the number of media samples in a sample buffer.

func CMSampleBufferGetTotalSampleSize(CMSampleBuffer) -> Int

Returns the total size in bytes of sample data in a sample buffer.

func CMSampleBufferGetSampleSize(CMSampleBuffer, at: CMItemIndex) -> Int

Returns the size in bytes of a specified sample in a sample buffer.

func CMSampleBufferGetSampleSizeArray(CMSampleBuffer, entryCount: CMItemCount, arrayToFill: UnsafeMutablePointer&lt;Int>?, entriesNeededOut: UnsafeMutablePointer&lt;CMItemCount>?) -> OSStatus

Retrieves an array of sample sizes that represents each sample in a sample buffer.

### Inspecting Duration and Timing

func CMSampleBufferGetDuration(CMSampleBuffer) -> CMTime

Returns the total duration of a sample buffer.

func CMSampleBufferGetDecodeTimeStamp(CMSampleBuffer) -> CMTime

Returns the decode timestamp that’s the earliest numerically of all the samples in a sample buffer.

func CMSampleBufferGetPresentationTimeStamp(CMSampleBuffer) -> CMTime

Returns the presentation timestamp that’s the earliest numerically of all the samples in a sample buffer.

func CMSampleBufferGetOutputDuration(CMSampleBuffer) -> CMTime

Returns the output duration of a sample buffer.

func CMSampleBufferGetOutputDecodeTimeStamp(CMSampleBuffer) -> CMTime

Returns the output decode timestamp of a sample buffer.

func CMSampleBufferGetOutputPresentationTimeStamp(CMSampleBuffer) -> CMTime

Returns the output presentation timestamp of a sample buffer.

func CMSampleBufferSetOutputPresentationTimeStamp(CMSampleBuffer, newValue: CMTime) -> OSStatus

Sets an output presentation timestamp to use in place of a calculated value.

func CMSampleBufferGetSampleTimingInfo(CMSampleBuffer, at: CMItemIndex, timingInfoOut: UnsafeMutablePointer&lt;CMSampleTimingInfo>) -> OSStatus

Retrieves a timing information structure that describes a specified sample in a sample buffer.

func CMSampleBufferGetSampleTimingInfoArray(CMSampleBuffer, entryCount: CMItemCount, arrayToFill: UnsafeMutablePointer&lt;CMSampleTimingInfo>?, entriesNeededOut: UnsafeMutablePointer&lt;CMItemCount>?) -> OSStatus

Retrieves an array of sample timing information structures that represents each sample in a sample buffer.

func CMSampleBufferGetOutputSampleTimingInfoArray(CMSampleBuffer, entryCount: CMItemCount, arrayToFill: UnsafeMutablePointer&lt;CMSampleTimingInfo>?, entriesNeededOut: UnsafeMutablePointer&lt;CMItemCount>?) -> OSStatus

Retrieves an array of output timing information structures that represents each sample in a sample buffer.

### Accessing the Format Description

func CMSampleBufferGetFormatDescription(CMSampleBuffer) -> CMFormatDescription?

Returns the format description of the samples in a sample buffer.

### Modifying Sample Buffers

func CMSampleBufferGetDataBuffer(CMSampleBuffer) -> CMBlockBuffer?

Returns a block buffer that contains the media data.

func CMSampleBufferSetDataBuffer(CMSampleBuffer, newValue: CMBlockBuffer) -> OSStatus

Sets a block buffer of media data on a sample buffer.

func CMSampleBufferGetImageBuffer(CMSampleBuffer) -> CVImageBuffer?

Returns an image buffer that contains the media data.

func CMSampleBufferGetAudioBufferListWithRetainedBlockBuffer(CMSampleBuffer, bufferListSizeNeededOut: UnsafeMutablePointer&lt;Int>?, bufferListOut: UnsafeMutablePointer&lt;AudioBufferList>?, bufferListSize: Int, blockBufferAllocator: CFAllocator?, blockBufferMemoryAllocator: CFAllocator?, flags: UInt32, blockBufferOut: UnsafeMutablePointer&lt;CMBlockBuffer?>?) -> OSStatus

Returns an audio buffer list that contains the media data.

func CMSampleBufferSetDataBufferFromAudioBufferList(CMSampleBuffer, blockBufferAllocator: CFAllocator?, blockBufferMemoryAllocator: CFAllocator?, flags: UInt32, bufferList: UnsafePointer&lt;AudioBufferList>) -> OSStatus

Creates a block buffer that contains a copy of the data from an audio buffer list.

func CMSampleBufferCopyPCMDataIntoAudioBufferList(CMSampleBuffer, at: Int32, frameCount: Int32, into: UnsafeMutablePointer&lt;AudioBufferList>) -> OSStatus

Copies PCM audio data from a sample buffer into an audio buffer list.

func CMSampleBufferGetAudioStreamPacketDescriptions(CMSampleBuffer, allocatedSize: Int, packetDescriptionsOut: UnsafeMutablePointer&lt;AudioStreamPacketDescription>?, packetDescriptionsSizeNeededOut: UnsafeMutablePointer&lt;Int>?) -> OSStatus

Creates an array of audio stream packet descriptions.

func CMSampleBufferGetAudioStreamPacketDescriptionsPtr(CMSampleBuffer, packetDescriptionsPointerOut: UnsafeMutablePointer&lt;UnsafePointer&lt;AudioStreamPacketDescription>?>?, sizeOut: UnsafeMutablePointer&lt;Int>?) -> OSStatus

Returns a pointer to a constant array of audio stream packet descriptions.

### Managing Attachments

func CMSampleBufferGetSampleAttachmentsArray(CMSampleBuffer, createIfNecessary: Bool) -> CFArray?

Retrieves an array of sample attachment dictionaries that represents each sample in a sample buffer.

Sample Attachment Keys

Keys that specify attachments to individual samples in a buffer.

### Processing Samples

func CMSampleBufferCallBlockForEachSample(CMSampleBuffer, (CMSampleBuffer, CMItemCount) -> OSStatus) -> OSStatus

Calls a block for every individual sample in a sample buffer.

func CMSampleBufferCallForEachSample(CMSampleBuffer, callback: (CMSampleBuffer, CMItemCount, UnsafeMutableRawPointer?) -> OSStatus, refcon: UnsafeMutableRawPointer?) -> OSStatus

Calls a function for every individual sample in a sample buffer.

### Accessing the Type Identifier

func CMSampleBufferGetTypeID() -> CFTypeID

Returns the type identifier of sample buffer objects.

### Data Types

class CMSampleBuffer

A reference to a buffer of media data.

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

### Notifications

Sample Buffer Notifications

Notifications the system posts when processing sample buffer objects.

### Errors

Sample Buffer Error Codes

Errors that occur when processing sample buffer objects.

var kCMPersistentTrackID_Invalid: CMPersistentTrackID

Indicates an invalid track ID.

### Functions

func CMTimeFoldIntoRange(CMTime, foldRange: CMTimeRange) -> CMTime

Folds a time into a time range.

func CMVideoFormatDescriptionGetHEVCParameterSetAtIndex(CMFormatDescription, parameterSetIndex: Int, parameterSetPointerOut: UnsafeMutablePointer&lt;UnsafePointer&lt;UInt8>?>?, parameterSetSizeOut: UnsafeMutablePointer&lt;Int>?, parameterSetCountOut: UnsafeMutablePointer&lt;Int>?, nalUnitHeaderLengthOut: UnsafeMutablePointer&lt;Int32>?) -> OSStatus

Returns a parameter set contained in an HEVC (H.265) format description.

## See Also

### Sample Processing

CMBlockBuffer APIs

An object the system uses to move blocks of memory through a processing system.

struct CMTaggedBuffer

An instance of a media buffer containing metadata tags.

CMTaggedBufferGroup APIs

Objective-C types and interfaces for working with Core Media tagged buffer groups.

CMFormatDescription APIs

A media format descriptor that describes the samples in a sample buffer.

CMAttachment APIs

Add supporting metadata to sample buffers.

