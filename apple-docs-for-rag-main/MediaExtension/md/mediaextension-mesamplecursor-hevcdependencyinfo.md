

- MediaExtension
- MESampleCursor
-  hevcDependencyInfo 

Instance Property

# hevcDependencyInfo

Additional information that’s necessary to recover complete sample dependency information.

macOS 14.0+

``` source
@NSCopying
optional var hevcDependencyInfo: MEHEVCDependencyInfo { get }
```

## Discussion

This is an optional property that provides additional sample dependency information that syncInfo and dependencyInfo don’t provide. Examples of this are the NAL unit type of an HEVC sync sample or the number of samples necessary to refresh the decoder after a USAC independent frame. Don’t implement this property for formats where this information doesn’t make sense.

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

var decodeTimeOfLastSampleReachableByForwardSteppingThatIsAlreadyLoadedByByteSource: CMTime

The duration of the playable content starting from the cursor position.

