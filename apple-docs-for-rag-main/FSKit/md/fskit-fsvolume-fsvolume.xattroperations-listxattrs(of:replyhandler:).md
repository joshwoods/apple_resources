

- FSKit
- FSVolume
- FSVolume.XattrOperations
-  listXattrs(of:replyHandler:) 

Instance Method

# listXattrs(of:replyHandler:)

Gets the list of extended attributes currently set on the given item.

macOS 15.4+

``` source
func listXattrs(
    of item: FSItem,
    replyHandler reply: @escaping ([FSFileName]?, (any Error)?) -> Void
)
```

``` source
func xattrs(of item: FSItem) async throws -> [FSFileName]
```

**Required**

## Parameters 

`item`  

The item from which to get extended attributes.

`reply`  

A block or closure to indicate success or failure. If getting the list of extended attributes succeeds, pass the xattrs as an array of FSFileName instances and a `nil` error. If getting the attriubtes fails, pass `nil` along with the relevant error. For an `async` Swift implementation, there’s no reply handler; simply return the byte count or throw an error.

## See Also

### Reading and writing

func getXattr(named: FSFileName, of: FSItem, replyHandler: (Data?, (any Error)?) -> Void)

Gets the specified extended attribute of the given item.

**Required**

func setXattr(named: FSFileName, to: Data?, on: FSItem, policy: FSVolume.SetXattrPolicy, replyHandler: ((any Error)?) -> Void)

Sets the specified extended attribute data on the given item.

**Required**

enum SetXattrPolicy

Flags to specify the policy when setting extended file attributes.

func supportedXattrNames(for: FSItem) -> [FSFileName]

Returns an array that specifies the extended attribute names the given item supports.

