

- AVFoundation
- AVSampleCursorSyncInfo
-  sampleIsFullSync 

Instance Property

# sampleIsFullSync

A Boolean value that indicates whether a sample is a full sync sample.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var sampleIsFullSync: ObjCBool
```

## Discussion

A full sync sample, also called a Instantaneous Decoder Refresh sample, is sufficient in itself to completely resynchronize a decoder.

## See Also

### Sync Information

var sampleIsPartialSync: ObjCBool

A Boolean value that indicates whether a sample is a partial sync sample.

var sampleIsDroppable: ObjCBool

A Boolean value that indicates whether a sample is droppable.

