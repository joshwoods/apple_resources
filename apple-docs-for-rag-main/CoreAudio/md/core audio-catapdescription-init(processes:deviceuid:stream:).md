

- Core Audio
- CATapDescription
-  init(processes:deviceUID:stream:) 

Initializer

# init(processes:deviceUID:stream:)

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
convenience init(
    processes processesIDsToIncludeInTap: [AudioObjectID],
    deviceUID: String,
    stream: UInt
)
```

## See Also

### Initializers

init()

convenience init(excludingProcesses: [AudioObjectID], deviceUID: String, stream: UInt)

convenience init(monoGlobalTapButExcludeProcesses: [AudioObjectID])

convenience init(monoMixdownOfProcesses: [AudioObjectID])

convenience init(stereoGlobalTapButExcludeProcesses: [AudioObjectID])

convenience init(stereoMixdownOfProcesses: [AudioObjectID])

