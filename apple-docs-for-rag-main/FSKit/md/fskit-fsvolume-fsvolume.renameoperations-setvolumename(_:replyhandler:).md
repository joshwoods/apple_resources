

- FSKit
- FSVolume
- FSVolume.RenameOperations
-  setVolumeName(\_:replyHandler:) 

Instance Method

# setVolumeName(\_:replyHandler:)

Sets a new name for the volume.

macOS 15.4+

``` source
func setVolumeName(
    _ name: FSFileName,
    replyHandler reply: @escaping (FSFileName, (any Error)?) -> Void
)
```

``` source
func setVolumeName(_ name: FSFileName) async throws -> FSFileName
```

**Required**

## Parameters 

`name`  

The new volume name.

`reply`  

A block or closure to indicate success or failure. If renaming succeeds, pass an FSFileName of the new volume name and a `nil` error. If renaming fails, pass the relevant error as the second parameter; FSKit ignores any FSFileName in this case. For an `async` Swift implementation, there’s no reply handler; simply return the FSFileName or throw an error.

