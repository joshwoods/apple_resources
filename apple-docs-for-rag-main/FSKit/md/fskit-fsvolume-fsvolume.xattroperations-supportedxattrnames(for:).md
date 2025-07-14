

- FSKit
- FSVolume
- FSVolume.XattrOperations
-  supportedXattrNames(for:) 

Instance Method

# supportedXattrNames(for:)

Returns an array that specifies the extended attribute names the given item supports.

macOS 15.4+

``` source
optional func supportedXattrNames(for item: FSItem) -> [FSFileName]
```

## Parameters 

`item`  

The item for which to get information.

## Discussion

If `item` supports no extended attributes, this method returns `nil`.

Only implement this method if your volume works with “limited” extended attributes. For purposes of this protocol, “limited” support means the volume doesn’t support extended attributes generally, but uses these APIs to expose specific file system data.

Note

If a file system implements this method, FSKit assumes limited support for extended attributes exists. In this mode, FSkit only calls this protocol’s methods for the extended attribute names this method returns.

## See Also

### Reading and writing

func getXattr(named: FSFileName, of: FSItem, replyHandler: (Data?, (any Error)?) -> Void)

Gets the specified extended attribute of the given item.

**Required**

func listXattrs(of: FSItem, replyHandler: ([FSFileName]?, (any Error)?) -> Void)

Gets the list of extended attributes currently set on the given item.

**Required**

func setXattr(named: FSFileName, to: Data?, on: FSItem, policy: FSVolume.SetXattrPolicy, replyHandler: ((any Error)?) -> Void)

Sets the specified extended attribute data on the given item.

**Required**

enum SetXattrPolicy

Flags to specify the policy when setting extended file attributes.

