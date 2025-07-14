

- Core Media
- CMSampleBuffer
-  CMSampleBuffer.PerSampleAttachmentsDictionary 

Structure

# CMSampleBuffer.PerSampleAttachmentsDictionary

A structure that defines keys to identify per-sample attachments.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct PerSampleAttachmentsDictionary
```

## Topics

### Specifying Keys

struct Key

### Accessing Elements

subscript(CMSampleBuffer.PerSampleAttachmentsDictionary.Key) -> Any?

## Relationships

### Conforms To

- Sequence

## See Also

### Managing Attachments

struct AttachmentKey

Keys that identify sample buffer attachments.

var sampleAttachments: CMSampleBuffer.SampleAttachmentsArray

An array of sample attachments.

struct SampleAttachmentsArray

A structure that defines an array of sample attachments.

