

- FSKit
- FSDirectoryEntryPacker
-  packEntry(name:itemType:itemID:nextCookie:attributes:) 

Instance Method

# packEntry(name:itemType:itemID:nextCookie:attributes:)

Provides a directory entry during enumeration.

macOS 15.4+

``` source
func packEntry(
    name: FSFileName,
    itemType: FSItem.ItemType,
    itemID: FSItem.Identifier,
    nextCookie: FSDirectoryCookie,
    attributes: FSItem.Attributes?
) -> Bool
```

## Parameters 

`name`  

The item’s name.

`itemType`  

The type of the item.

`itemID`  

The item’s identifier.

`nextCookie`  

A value to indicate the next entry in the directory to enumerate. FSKit passes this value as the `cookie` parameter on the next call to enumerateDirectory(_:startingAt:verifier:attributes:packer:replyHandler:). Use whatever value is appropriate for your implementation; the value is opaque to FSKit.

`attributes`  

The item’s attributes. Pass `nil` if the enumeration call didn’t request attributes.

## Return Value

`true` (Swift) or `YES` (Objective-C) if packing was successful and enumeration can continue with the next directory entry. If the value is `false` (Swift) or `NO` (Objective-C), stop enumerating. This result can happen when the entry is too big for the remaining space in the buffer.

## Discussion

You call this method in your implementation of enumerateDirectory(_:startingAt:verifier:attributes:packer:replyHandler:), for each directory entry you want to provide to the enumeration.

