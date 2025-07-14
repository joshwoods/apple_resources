

- Core Foundation
-  CFTreeGetChildAtIndex(\_:\_:) 

Function

# CFTreeGetChildAtIndex(\_:\_:)

Returns the child of a tree at the specified index.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFTreeGetChildAtIndex(
    _ tree: CFTree!,
    _ idx: CFIndex
) -> CFTree!
```

## Parameters 

`tree`  

The tree to examine.

`idx`  

The index of the child obtain. The value must be less than the number of children in `tree`.

## Return Value

The child tree at `idx`. Ownership follows the The Get Rule.

## See Also

### Examining a Tree

func CFTreeFindRoot(CFTree!) -> CFTree!

Returns the root tree of a given tree.

func CFTreeGetChildCount(CFTree!) -> CFIndex

Returns the number of children in a tree.

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

