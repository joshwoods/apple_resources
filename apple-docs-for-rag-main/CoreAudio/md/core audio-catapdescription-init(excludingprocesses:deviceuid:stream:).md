

- Core Audio
- CATapDescription
-  init(excludingProcesses:deviceUID:stream:) 

Initializer

# init(excludingProcesses:deviceUID:stream:)

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
convenience init(
    excludingProcesses processesIDsToExcludeFromTap: [AudioObjectID],
    deviceUID: String,
    stream: UInt
)
```

## See Also

### Initializers

init()

convenience init(monoGlobalTapButExcludeProcesses: [AudioObjectID])

convenience init(monoMixdownOfProcesses: [AudioObjectID])

convenience init(processes: [AudioObjectID], deviceUID: String, stream: UInt)

convenience init(stereoGlobalTapButExcludeProcesses: [AudioObjectID])

convenience init(stereoMixdownOfProcesses: [AudioObjectID])

