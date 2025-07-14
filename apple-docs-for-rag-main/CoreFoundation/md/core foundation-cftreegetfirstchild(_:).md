

- Core Foundation
-  CFTreeGetFirstChild(\_:) 

Function

# CFTreeGetFirstChild(\_:)

Returns the first child of a tree.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFTreeGetFirstChild(_ tree: CFTree!) -> CFTree!
```

## Parameters 

`tree`  

The tree to examine.

## Return Value

The first child of `tree`. Ownership follows the The Get Rule.

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

func CFTreeGetContext(CFTree!, UnsafeMutablePointer&lt;CFTreeContext>!)

Returns the context of the specified tree.

func CFTreeGetNextSibling(CFTree!) -> CFTree!

Returns the next sibling, adjacent to a given tree, in the parent’s children list.

func CFTreeGetParent(CFTree!) -> CFTree!

Returns the parent of a given tree.

