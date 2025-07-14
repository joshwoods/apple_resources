

- FSKit
- FSVolume
- FSVolume.XattrOperations
-  setXattr(named:to:on:policy:replyHandler:) 

Instance Method

# setXattr(named:to:on:policy:replyHandler:)

Sets the specified extended attribute data on the given item.

macOS 15.4+

``` source
func setXattr(
    named name: FSFileName,
    to value: Data?,
    on item: FSItem,
    policy: FSVolume.SetXattrPolicy,
    replyHandler reply: @escaping ((any Error)?) -> Void
)
```

``` source
func setXattr(
    named name: FSFileName,
    to value: Data?,
    on item: FSItem,
    policy: FSVolume.SetXattrPolicy
) async throws
```

**Required**

## Parameters 

`name`  

The extended attribute name.

`value`  

The extended attribute value to set. This can’t be `nil`, unless the policy is FSVolume.SetXattrPolicy.delete.

`item`  

The item on which to set the extended attribute.

`policy`  

The policy to apply when setting the attribute. See FSVolume.SetXattrPolicy for possible values.

`reply`  

A block or closure to indicate success or failure. If setting the attribute fails, pass an error as the one parameter to the reply handler. If setting the attribute succeeds, pass `nil`. For an `async` Swift implementation, there’s no reply handler; simply throw an error or return normally.

## See Also

### Reading and writing

func getXattr(named: FSFileName, of: FSItem, replyHandler: (Data?, (any Error)?) -> Void)

Gets the specified extended attribute of the given item.

**Required**

func listXattrs(of: FSItem, replyHandler: ([FSFileName]?, (any Error)?) -> Void)

Gets the list of extended attributes currently set on the given item.

**Required**

enum SetXattrPolicy

Flags to specify the policy when setting extended file attributes.

func supportedXattrNames(for: FSItem) -> [FSFileName]

Returns an array that specifies the extended attribute names the given item supports.

