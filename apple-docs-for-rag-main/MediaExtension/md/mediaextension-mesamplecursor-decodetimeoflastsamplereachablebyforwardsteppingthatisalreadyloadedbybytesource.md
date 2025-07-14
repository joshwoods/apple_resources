

- MediaExtension
- MESampleCursor
-  decodeTimeOfLastSampleReachableByForwardSteppingThatIsAlreadyLoadedByByteSource 

Instance Property

# decodeTimeOfLastSampleReachableByForwardSteppingThatIsAlreadyLoadedByByteSource

The duration of the playable content starting from the cursor position.

macOS 14.0+

``` source
optional var decodeTimeOfLastSampleReachableByForwardSteppingThatIsAlreadyLoadedByByteSource: CMTime { get }
```

## Discussion

Indicates the time difference between the current cursor decode timestamp (DTS) and the last reachable sample DTS. This is necessary to play certain assets such as those with HTTP URLs, because it indicates what samples the byte source has already loaded.

## See Also

### Inspecting a sample cursor

var presentationTimeStamp: CMTime

The presentation timestamp (PTS) of the sample at the current position of the cursor.

**Required**

var decodeTimeStamp: CMTime

The decode timestamp (DTS) of the sample at the current position of the cursor.

**Required**

var currentSampleDuration: CMTime

The decode duration of the sample at the current position.

**Required**

var currentSampleFormatDescription: CMFormatDescription?

The format description for the sample at the current position of the cursor.

**Required**

var syncInfo: AVSampleCursorSyncInfo

Decoder synchronization information about the sample the cursor points to.

var dependencyInfo: AVSampleCursorDependencyInfo

Dependency information about the sample the cursor points to.

var hevcDependencyInfo: MEHEVCDependencyInfo

Additional information that’s necessary to recover complete sample dependency information.

