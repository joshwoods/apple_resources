

- FSKit
- FSVolume
- FSVolume.ItemDeactivation
-  deactivateItem(\_:replyHandler:) 

Instance Method

# deactivateItem(\_:replyHandler:)

Notifies the file system that the kernel is no longer making immediate use of the given item.

macOS 15.4+

``` source
func deactivateItem(
    _ item: FSItem,
    replyHandler reply: @escaping ((any Error)?) -> Void
)
```

``` source
func deactivateItem(_ item: FSItem) async throws
```

**Required**

## Parameters 

`item`  

The item to deactivate.

`reply`  

A block or closure to indicate success or failure. If deactivation fails, pass an error as the one parameter to the reply handler. If deactivation succeeds, pass `nil`. For an `async` Swift implementation, there’s no reply handler; simply throw an error or return normally.

## Discussion

This method gives a file system a chance to release resources associated wtih an item. However, this method prescribes no specific action; it’s acceptable to defer all reclamation until reclaimItem(_:replyHandler:). This method is the equivalent of VFS’s `VNOP_INACTIVE`.

FSKit restricts calls to this method based on the current value of itemDeactivationPolicy.

