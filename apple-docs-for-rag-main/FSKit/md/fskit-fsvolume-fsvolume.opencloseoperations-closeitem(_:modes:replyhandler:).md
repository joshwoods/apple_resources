

- FSKit
- FSVolume
- FSVolume.OpenCloseOperations
-  closeItem(\_:modes:replyHandler:) 

Instance Method

# closeItem(\_:modes:replyHandler:)

Closes a file from further access.

macOS 15.4+

``` source
func closeItem(
    _ item: FSItem,
    modes: FSVolume.OpenModes,
    replyHandler reply: @escaping ((any Error)?) -> Void
)
```

``` source
func closeItem(
    _ item: FSItem,
    modes: FSVolume.OpenModes
) async throws
```

**Required**

## Parameters 

`item`  

The item to close.

`modes`  

The set of mode flags to keep after this close.

`reply`  

A block or closure to indicate success or failure. If closing fails, pass an error as the one parameter to the reply handler. If closing succeeds, pass `nil`. For an `async` Swift implementation, there’s no reply handler; simply throw an error or return normally.

## See Also

### Opening and closing

func openItem(FSItem, modes: FSVolume.OpenModes, replyHandler: ((any Error)?) -> Void)

Opens a file for access.

**Required**

struct OpenModes

Defined modes for opening a file.

