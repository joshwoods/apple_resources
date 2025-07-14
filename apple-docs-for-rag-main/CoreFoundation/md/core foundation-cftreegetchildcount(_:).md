

- Core Foundation
-  CFTreeGetChildCount(\_:) 

Function

# CFTreeGetChildCount(\_:)

Returns the number of children in a tree.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFTreeGetChildCount(_ tree: CFTree!) -> CFIndex
```

## Parameters 

`tree`  

The tree to examine.

## Return Value

The number of children in `tree`.

## See Also

### Examining a Tree

func CFTreeFindRoot(CFTree!) -> CFTree!

Returns the root tree of a given tree.

func CFTreeGetChildAtIndex(CFTree!, CFIndex) -> CFTree!

Returns the child of a tree at the specified index.

func CFTreeGetChildren(CFTree!, UnsafeMutablePointer&lt;Unmanaged&lt;CFTree>?>!)

Fills a buffer with children from the tree.

func CFTreeGetContext(CFTree!, UnsafeMutablePointer&lt;CFTreeContext>!)

Returns the context of the specified tree.

func CFTreeGetFirstChild(CFTree!) -> CFTree!

Returns the first child of a tree.

func CFTreeGetNextSibling(CFTree!) -> CFTree!

Returns the next sibling, adjacent to a given tree, in the parent’s children list.

func CFTreeGetParent(CFTree!) -> CFTree!

Returns the parent of a given tree.

