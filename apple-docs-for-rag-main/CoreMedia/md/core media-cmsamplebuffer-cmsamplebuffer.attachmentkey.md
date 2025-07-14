

- Core Media
- CMSampleBuffer
-  CMSampleBuffer.AttachmentKey 

Structure

# CMSampleBuffer.AttachmentKey

Keys that identify sample buffer attachments.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct AttachmentKey
```

## Topics

### Attachment Keys

static let cameraIntrinsicMatrix: CMSampleBuffer.AttachmentKey

static let displayEmptyMediaImmediately: CMSampleBuffer.AttachmentKey

static let drainAfterDecoding: CMSampleBuffer.AttachmentKey

static let droppedFrameReason: CMSampleBuffer.AttachmentKey

static let droppedFrameReasonInfo: CMSampleBuffer.AttachmentKey

static let emptyMedia: CMSampleBuffer.AttachmentKey

static let endsPreviousSampleDuration: CMSampleBuffer.AttachmentKey

static let fillDiscontinuitiesWithSilence: CMSampleBuffer.AttachmentKey

static let forceKeyFrame: CMSampleBuffer.AttachmentKey

static let gradualDecoderRefresh: CMSampleBuffer.AttachmentKey

static let permanentEmptyMedia: CMSampleBuffer.AttachmentKey

static let postNotificationWhenConsumed: CMSampleBuffer.AttachmentKey

static let resetDecoderBeforeDecoding: CMSampleBuffer.AttachmentKey

static let resumeOutput: CMSampleBuffer.AttachmentKey

static let reverse: CMSampleBuffer.AttachmentKey

static let sampleReferenceByteOffset: CMSampleBuffer.AttachmentKey

static let sampleReferenceURL: CMSampleBuffer.AttachmentKey

static let speedMultiplier: CMSampleBuffer.AttachmentKey

static let stillImageLensStabilizationInfo: CMSampleBuffer.AttachmentKey

static let transitionID: CMSampleBuffer.AttachmentKey

static let trimDurationAtEnd: CMSampleBuffer.AttachmentKey

static let trimDurationAtStart: CMSampleBuffer.AttachmentKey

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing Attachments

var sampleAttachments: CMSampleBuffer.SampleAttachmentsArray

An array of sample attachments.

struct SampleAttachmentsArray

A structure that defines an array of sample attachments.

struct PerSampleAttachmentsDictionary

A structure that defines keys to identify per-sample attachments.

