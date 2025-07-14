

- MediaExtension
- MESampleCursor
-  dependencyInfo 

Instance Property

# dependencyInfo

Dependency information about the sample the cursor points to.

macOS 14.0+

``` source
optional var dependencyInfo: AVSampleCursorDependencyInfo { get }
```

## Discussion

This value includes any valid flags set. Don’t implement this property if this kind of dependency information doesn’t make sense for the sequence of samples.

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

var hevcDependencyInfo: MEHEVCDependencyInfo

Additional information that’s necessary to recover complete sample dependency information.

var decodeTimeOfLastSampleReachableByForwardSteppingThatIsAlreadyLoadedByByteSource: CMTime

The duration of the playable content starting from the cursor position.

