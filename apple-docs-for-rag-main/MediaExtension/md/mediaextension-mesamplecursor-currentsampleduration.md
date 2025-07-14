

- MediaExtension
- MESampleCursor
-  currentSampleDuration 

Instance Property

# currentSampleDuration

The decode duration of the sample at the current position.

macOS 14.0+

``` source
var currentSampleDuration: CMTime { get }
```

**Required**

## Discussion

This value is indefinite if the system needs to advance the sample past its current position to determine the decode duration. This can occur with streaming formats such as MPEG-2 transport streams.

## See Also

### Inspecting a sample cursor

var presentationTimeStamp: CMTime

The presentation timestamp (PTS) of the sample at the current position of the cursor.

**Required**

var decodeTimeStamp: CMTime

The decode timestamp (DTS) of the sample at the current position of the cursor.

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

var decodeTimeOfLastSampleReachableByForwardSteppingThatIsAlreadyLoadedByByteSource: CMTime

The duration of the playable content starting from the cursor position.

