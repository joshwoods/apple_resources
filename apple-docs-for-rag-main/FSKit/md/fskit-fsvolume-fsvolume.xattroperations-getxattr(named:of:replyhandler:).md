

- FSKit
- FSVolume
- FSVolume.XattrOperations
-  getXattr(named:of:replyHandler:) 

Instance Method

# getXattr(named:of:replyHandler:)

Gets the specified extended attribute of the given item.

macOS 15.4+

``` source
func getXattr(
    named name: FSFileName,
    of item: FSItem,
    replyHandler reply: @escaping (Data?, (any Error)?) -> Void
)
```

``` source
func xattr(
    named name: FSFileName,
    of item: FSItem
) async throws -> Data
```

**Required**

## Parameters 

`name`  

The extended attribute name.

`item`  

The item for which to get the extended attribute.

`reply`  

A block or closure to indicate success or failure. If getting the attribute succeeds, pass an data instance containing the extended attribute data and a `nil` error. If getting the attribute fails, pass the relevant error as the second parameter; FSKit ignores any data in this case. For an `async` Swift implementation, there’s no reply handler; simply return the data or throw an error.

## See Also

### Reading and writing

func listXattrs(of: FSItem, replyHandler: ([FSFileName]?, (any Error)?) -> Void)

Gets the list of extended attributes currently set on the given item.

**Required**

func setXattr(named: FSFileName, to: Data?, on: FSItem, policy: FSVolume.SetXattrPolicy, replyHandler: ((any Error)?) -> Void)

Sets the specified extended attribute data on the given item.

**Required**

enum SetXattrPolicy

Flags to specify the policy when setting extended file attributes.

func supportedXattrNames(for: FSItem) -> [FSFileName]

Returns an array that specifies the extended attribute names the given item supports.

