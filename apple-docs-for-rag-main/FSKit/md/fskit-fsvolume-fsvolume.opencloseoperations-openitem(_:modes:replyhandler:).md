

- FSKit
- FSVolume
- FSVolume.OpenCloseOperations
-  openItem(\_:modes:replyHandler:) 

Instance Method

# openItem(\_:modes:replyHandler:)

Opens a file for access.

macOS 15.4+

``` source
func openItem(
    _ item: FSItem,
    modes: FSVolume.OpenModes,
    replyHandler reply: @escaping ((any Error)?) -> Void
)
```

``` source
func openItem(
    _ item: FSItem,
    modes: FSVolume.OpenModes
) async throws
```

**Required**

## Parameters 

`item`  

The item to open.

`modes`  

The set of mode flags to open the item with.

`reply`  

A block or closure to indicate success or failure. If opening fails, pass an error as the one parameter to the reply handler. If opening succeeds, pass `nil`. For an `async` Swift implementation, there’s no reply handler; simply throw an error or return normally.

## See Also

### Opening and closing

func closeItem(FSItem, modes: FSVolume.OpenModes, replyHandler: ((any Error)?) -> Void)

Closes a file from further access.

**Required**

struct OpenModes

Defined modes for opening a file.

