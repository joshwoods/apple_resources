

- Core Media
-  kCMSampleAttachmentKey_HasRedundantCoding 

Global Variable

# kCMSampleAttachmentKey_HasRedundantCoding

Indicates whether the sample has redundant coding (type `CFBoolean`).

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
let kCMSampleAttachmentKey_HasRedundantCoding: CFString
```

## Discussion

This key has no default value. If this key is not present, redundant coding information for the sample is unknown.

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

let kCMSampleAttachmentKey_DoNotDisplay: CFString

Indicates whether the sample should be decoded but not displayed (type `CFBoolean`, default false).

let kCMSampleAttachmentKey_EarlierDisplayTimesAllowed: CFString

Indicates whether later samples may have earlier display times (type `CFBoolean`).

let kCMSampleAttachmentKey_PostDecodeProcessingMetadata: CFString

