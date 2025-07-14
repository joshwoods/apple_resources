

- Core Media
-  kCMSampleAttachmentKey_PostDecodeProcessingMetadata 

Global Variable

# kCMSampleAttachmentKey_PostDecodeProcessingMetadata

macOS 15.0+

``` source
let kCMSampleAttachmentKey_PostDecodeProcessingMetadata: CFString
```

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

let kCMSampleAttachmentKey_HasRedundantCoding: CFString

Indicates whether the sample has redundant coding (type `CFBoolean`).

