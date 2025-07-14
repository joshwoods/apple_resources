

- FSKit
- FSVolume
- FSVolume.Operations
-  enumerateDirectory(\_:startingAt:verifier:attributes:packer:replyHandler:) 

Instance Method

# enumerateDirectory(\_:startingAt:verifier:attributes:packer:replyHandler:)

Enumerates the contents of the given directory.

macOS 15.4+

``` source
func enumerateDirectory(
    _ directory: FSItem,
    startingAt cookie: FSDirectoryCookie,
    verifier: FSDirectoryVerifier,
    attributes: FSItem.GetAttributesRequest?,
    packer: FSDirectoryEntryPacker,
    replyHandler reply: @escaping (FSDirectoryVerifier, (any Error)?) -> Void
)
```

``` source
func enumerateDirectory(
    _ directory: FSItem,
    startingAt cookie: FSDirectoryCookie,
    verifier: FSDirectoryVerifier,
    attributes: FSItem.GetAttributesRequest?,
    packer: FSDirectoryEntryPacker
) async throws -> FSDirectoryVerifier
```

**Required**

## Parameters 

`directory`  

The item to enumerate. FSKit guarantees this item is of type FSItem.ItemType.directory.

`cookie`  

A value that indicates the location within the directory from which to enumerate. Your implementation defines the semantics of the cookie values; they’re opaque to FSKit. The first call to the enumerate method passes initial for this parameter. Subsequent calls pass whatever cookie value you previously passed to the packer’s `nextCookie` parmeter.

`verifier`  

A tool to detect whether the directory contents changed since the last call to `enumerateDirectory`. Your implementation defines the semantics of the verifier values; they’re opaque to FSKit. The first call to the enumerate method passes initial for this parameter. Subsequent calls pass whatever cookie value you previously passed to the packer’s `currentVerifier` parmeter.

`attributes`  

The desired attributes to provide, or `nil` if the caller doesn’t require attributes.

`packer`  

An object that your implementation uses to enumerate directory items, packing one item per callback to `enumerateDirectory`.

`reply`  

A block or closure to indicate success or failure. If enumeration succeeds, pass the current verifier and a `nil` error. If enumeration fails, pass the relevant error as the second parameter; FSKit ignores any verifier in this case. For an `async` Swift implementation, there’s no reply handler; simply return the current verifier or throw an error.

## Discussion

This method uses the packEntry(name:itemType:itemID:nextCookie:attributes:) method of the `packer` parameter to deliver the enumerated items to the caller. The general flow of an enumeration implementation follows these steps:

1.  Enumeration starts with a call to `enumerateDirectory` using the initial next-cookie and verifier values initial and initial, respectively.

2.  The implementation uses `packer` to pack the initial set of directory entries. Packing also sets a `nextCookie` to use on the next call.

3.  The implementation replies with a new verifier value, a nonzero value that reflects the directory’s current version.

4.  On the next call the implementation packs the next set of entries, starting with the item indicated by `cookie`. If `cookie` doesn’t resolve to a valid directory entry, complete the request with an error of domain NSPOSIXErrorDomain and code FSError.Code.invalidDirectoryCookie.

When packing, make sure to use acceptable directory entry names and unambiguous input to all file operations that take names without additional normalization, such as`lookupName`.

Tip

If the `attributes` parameter is `nil`, include at least two entries in a directory: `"."` and `".."`, which represent the current and parent directories, respectively. Both of these items have type FSItem.ItemType.directory. For the root directory, `"."` and `".."` have identical contents. Don’t pack `"."` and `".."` if `attributes` isn’t `nil`.

## See Also

### Inspecting directory contents

struct FSDirectoryCookie

A value that indicates a location in a directory from which to enumerate.

struct FSDirectoryCookie

A value that indicates a location in a directory from which to enumerate.

struct FSDirectoryVerifier

A tool to detect whether the directory contents changed since the last call to enumerate a directory.

struct FSDirectoryVerifier

A tool to detect whether the directory contents changed since the last call to enumerate a directory.

class FSDirectoryEntryPacker

An object used to provide items during a directory enumeration.

