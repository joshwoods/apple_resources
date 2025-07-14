

- FSKit
- FSVolume
- FSVolume.Operations
-  getAttributes(\_:of:replyHandler:) 

Instance Method

# getAttributes(\_:of:replyHandler:)

Fetches attributes for the given item.

macOS 15.4+

``` source
func getAttributes(
    _ desiredAttributes: FSItem.GetAttributesRequest,
    of item: FSItem,
    replyHandler reply: @escaping (FSItem.Attributes?, (any Error)?) -> Void
)
```

``` source
func attributes(
    _ desiredAttributes: FSItem.GetAttributesRequest,
    of item: FSItem
) async throws -> FSItem.Attributes
```

**Required**

## Parameters 

`desiredAttributes`  

A requested set of attributes to get. The implementation inspects the request’s wantedAttributes to determine which attributes to populate.

`item`  

The item to get attributes for.

`reply`  

A block or closure to indicate success or failure. If getting attributes succeeds, pass an FSItem.Attributes with the requested attributes populated and a `nil` error. If getting attributes fails, pass the relevant error as the second parameter; FSKit ignores any FSItem.Attributes in this case. For an `async` Swift implementation, there’s no reply handler; simply return the FSItem.Attributes or throw an error.

## Discussion

For file systems that don’t support hard links, set linkCount to `1` for regular files and symbolic links.

If the item’s `bsdFlags` contain the `UF_COMPRESSED` flag, your file system returns the uncompressed size of the file.

## See Also

### Working with attributes

class GetAttributesRequest

A request to get attributes from an item.

func setAttributes(FSItem.SetAttributesRequest, on: FSItem, replyHandler: (FSItem.Attributes?, (any Error)?) -> Void)

Sets the given attributes on an item.

**Required**

class SetAttributesRequest

A request to set attributes on an item.

