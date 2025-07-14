

- Core Media
-  kCMSampleAttachmentKey_DependsOnOthers 

Global Variable

# kCMSampleAttachmentKey_DependsOnOthers

Indicates whether the sample depends on other samples for decoding (type `CFBoolean`).

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
let kCMSampleAttachmentKey_DependsOnOthers: CFString
```

## Discussion

This key has no default value. If this key is not present, dependency information for the sample is unknown. A value of kCFBooleanFalse indicates that the sample does not depend on other samples (for example, an I frame). A value of kCFBooleanTrue indicates that the sample does depend on other samples (for example, a P or B frame).

This attachment is read from and written to media files.

## See Also

### Sample Keys

let kCMSampleAttachmentKey_NotSync: CFString

Indicates whether the sample is a sync sample (type `CFBoolean`, default false).

let kCMSampleAttachmentKey_PartialSync: CFString

Indicates whether the sample is a partial sync sample (type `CFBoolean`, default false).

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

let kCMSampleAttachmentKey_PostDecodeProcessingMetadata: CFString

