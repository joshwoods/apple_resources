

- AVFoundation
- AVSampleCursorStorageRange
-  init(offset:length:) 

Initializer

# init(offset:length:)

Creates a storage range structure with offset and length values.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    offset: Int64,
    length: Int64
)
```

## Parameters 

`offset`  

The offset of the first byte of storage that a media sample or its chunk occupies.

`length`  

The number of storage bytes that a media sample or its chunk occupies.

