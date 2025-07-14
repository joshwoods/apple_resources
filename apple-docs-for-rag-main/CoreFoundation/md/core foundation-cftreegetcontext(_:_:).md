

- Core Foundation
-  CFTreeGetContext(\_:\_:) 

Function

# CFTreeGetContext(\_:\_:)

Returns the context of the specified tree.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFTreeGetContext(
    _ tree: CFTree!,
    _ context: UnsafeMutablePointer!
)
```

## Parameters 

`tree`  

The tree to examine.

`context`  

The CFTreeContext structure to be filled in with the context of the specified tree. This value must be a valid C pointer to a CFTreeContext structure-sized block of storage. If the version number of the storage is not a valid CFTreeContext structure version number, the result is undefined.

## See Also

### Examining a Tree

func CFTreeFindRoot(CFTree!) -> CFTree!

Returns the root tree of a given tree.

func CFTreeGetChildAtIndex(CFTree!, CFIndex) -> CFTree!

Returns the child of a tree at the specified index.

func CFTreeGetChildCount(CFTree!) -> CFIndex

Returns the number of children in a tree.

func CFTreeGetChildren(CFTree!, UnsafeMutablePointer&lt;Unmanaged&lt;CFTree>?>!)

Fills a buffer with children from the tree.

func CFTreeGetFirstChild(CFTree!) -> CFTree!

Returns the first child of a tree.

func CFTreeGetNextSibling(CFTree!) -> CFTree!

Returns the next sibling, adjacent to a given tree, in the parent’s children list.

func CFTreeGetParent(CFTree!) -> CFTree!

Returns the parent of a given tree.

