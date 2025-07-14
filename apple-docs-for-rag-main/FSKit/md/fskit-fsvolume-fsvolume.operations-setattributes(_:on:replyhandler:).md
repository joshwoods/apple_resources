

- FSKit
- FSVolume
- FSVolume.Operations
-  setAttributes(\_:on:replyHandler:) 

Instance Method

# setAttributes(\_:on:replyHandler:)

Sets the given attributes on an item.

macOS 15.4+

``` source
func setAttributes(
    _ newAttributes: FSItem.SetAttributesRequest,
    on item: FSItem,
    replyHandler reply: @escaping (FSItem.Attributes?, (any Error)?) -> Void
)
```

``` source
func setAttributes(
    _ newAttributes: FSItem.SetAttributesRequest,
    on item: FSItem
) async throws -> FSItem.Attributes
```

**Required**

## Parameters 

`newAttributes`  

A request containing the attributes to set.

`item`  

The item on which to set the attributes.

`reply`  

A block or closure to indicate success or failure. If setting attributes succeeds, pass an FSItem.Attributes with the item’s updated attributes and a `nil` error. If setting attributes fails, pass the relevant error as the second parameter; FSKit ignores any FSItem.Attributes in this case. For an `async` Swift implementation, there’s no reply handler; simply return the FSItem.Attributes or throw an error.

## Discussion

Several attributes are considered “read-only”, and an attempt to set these attributes results in an error with the code `EINVAL`.

A request may set size beyond the end of the file. If the underlying file system doesn’t support sparse files, allocate space to fill the new file size. Either fill this space with zeroes, or configure it to read as zeroes.

If a request sets the file size below the current end-of-file, truncate the file and return any unused space to the file system as free space.

Ignore attempts to set the size of directories or symbolic links; don’t produce an error.

If the caller attepts to sest an attribute not supported by the on-disk file system format, don’t produce an error. The upper layers of the framework will detect this situation.

## See Also

### Working with attributes

func getAttributes(FSItem.GetAttributesRequest, of: FSItem, replyHandler: (FSItem.Attributes?, (any Error)?) -> Void)

Fetches attributes for the given item.

**Required**

class GetAttributesRequest

A request to get attributes from an item.

class SetAttributesRequest

A request to set attributes on an item.

