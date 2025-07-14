

- Core Media
-  kCMSampleAttachmentKey_DoNotDisplay 

Global Variable

# kCMSampleAttachmentKey_DoNotDisplay

Indicates whether the sample should be decoded but not displayed (type `CFBoolean`, default false).

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
let kCMSampleAttachmentKey_DoNotDisplay: CFString
```

## Discussion

Use this attachment at run time to request this behavior from a display pipeline such as the AVSampleBufferDisplayLayer class.

This attachment is not written to media files.

## See Also

### Sample Keys

let kCMSampleAttachmentKey_NotSync: CFString

Indicates whether the sample is a sync sample (type `CFBoolean`, default false).

let kCMSampleAttachmentKey_PartialSync: CFString

Indicates whether the sample is a partial sync sample (type `CFBoolean`, default false).

let kCMSampleAttachmentKey_DependsOnOthers: CFString

Indicates whether the sample depends on other samples for decoding (type `CFBoolean`).

let kCMSampleAttachmentKey_IsDependedOnByOthers: CFString

Indicates whether other samples depend on this sample for decoding (type `CFBoolean`).

let kCMSampleAttachmentKey_DisplayImmediately: CFString

Indicates whether the sample should be displayed immediately (type `CFBoolean`, default false).

let kCMSampleAttachmentKey_EarlierDisplayTimesAllowed: CFString

Indicates whether later samples may have earlier display times (type `CFBoolean`).

let kCMSampleAttachmentKey_HasRedundantCoding: CFString

Indicates whether the sample has redundant coding (type `CFBoolean`).

let kCMSampleAttachmentKey_PostDecodeProcessingMetadata: CFString

