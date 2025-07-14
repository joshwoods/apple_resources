

- AVFoundation
- AVSampleCursorSyncInfo
-  init(sampleIsFullSync:sampleIsPartialSync:sampleIsDroppable:) 

Initializer

# init(sampleIsFullSync:sampleIsPartialSync:sampleIsDroppable:)

Creates a sample cursor sync information structure with media sample information.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    sampleIsFullSync: ObjCBool,
    sampleIsPartialSync: ObjCBool,
    sampleIsDroppable: ObjCBool
)
```

## Parameters 

`sampleIsFullSync`  

A Boolean value that indicates whether a sample is a full sync sample.

`sampleIsPartialSync`  

A Boolean value that indicates whether a sample is a partial sync sample.

`sampleIsDroppable`  

A Boolean value that indicates whether a sample is droppable.

