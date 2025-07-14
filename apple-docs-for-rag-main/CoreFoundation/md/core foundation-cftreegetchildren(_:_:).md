

- Core Foundation
-  CFTreeGetChildren(\_:\_:) 

Function

# CFTreeGetChildren(\_:\_:)

Fills a buffer with children from the tree.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFTreeGetChildren(
    _ tree: CFTree!,
    _ children: UnsafeMutablePointer?>!
)
```

## Parameters 

`tree`  

The tree to examine.

`children`  

The C array of pointer-sized values to be filled with the children from `tree`. This value must be a valid pointer to a C array of at least the size of the number of children in `tree`. Use the CFTreeGetChildCount(_:) function to obtain the number of children in `tree`. You are responsible for retaining and releasing the returned objects as needed.

## See Also

### Examining a Tree

func CFTreeFindRoot(CFTree!) -> CFTree!

Returns the root tree of a given tree.

func CFTreeGetChildAtIndex(CFTree!, CFIndex) -> CFTree!

Returns the child of a tree at the specified index.

func CFTreeGetChildCount(CFTree!) -> CFIndex

Returns the number of children in a tree.

func CFTreeGetContext(CFTree!, UnsafeMutablePointer&lt;CFTreeContext>!)

Returns the context of the specified tree.

func CFTreeGetFirstChild(CFTree!) -> CFTree!

Returns the first child of a tree.

func CFTreeGetNextSibling(CFTree!) -> CFTree!

Returns the next sibling, adjacent to a given tree, in the parent’s children list.

func CFTreeGetParent(CFTree!) -> CFTree!

Returns the parent of a given tree.

