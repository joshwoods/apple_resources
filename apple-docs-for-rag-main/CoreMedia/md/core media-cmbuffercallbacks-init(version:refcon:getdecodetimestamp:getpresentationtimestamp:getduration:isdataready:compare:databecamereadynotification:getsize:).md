

- Core Media
- CMBufferCallbacks
-  init(version:refcon:getDecodeTimeStamp:getPresentationTimeStamp:getDuration:isDataReady:compare:dataBecameReadyNotification:getSize:) 

Initializer

# init(version:refcon:getDecodeTimeStamp:getPresentationTimeStamp:getDuration:isDataReady:compare:dataBecameReadyNotification:getSize:)

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    version: UInt32,
    refcon: UnsafeMutableRawPointer?,
    getDecodeTimeStamp: CMBufferGetTimeCallback?,
    getPresentationTimeStamp: CMBufferGetTimeCallback?,
    getDuration: CMBufferGetTimeCallback,
    isDataReady: CMBufferGetBooleanCallback?,
    compare: CMBufferCompareCallback?,
    dataBecameReadyNotification: Unmanaged?,
    getSize: CMBufferGetSizeCallback?
)
```

