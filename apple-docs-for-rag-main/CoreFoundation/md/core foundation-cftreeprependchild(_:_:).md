

- Core Foundation
-  CFTreePrependChild(\_:\_:) 

Function

# CFTreePrependChild(\_:\_:)

Adds a new child to the specified tree as the first in its list of children.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFTreePrependChild(
    _ tree: CFTree!,
    _ newChild: CFTree!
)
```

## Parameters 

`tree`  

The tree to which to add `newChild`.

`newChild`  

The child tree to add to `tree`. This value must not be a child of another tree.

## Discussion

When a child tree is added to another tree, the child tree is retained by its new parent.

## See Also

### Modifying a Tree

func CFTreeAppendChild(CFTree!, CFTree!)

Adds a new child to a tree as the last in its list of children.

func CFTreeInsertSibling(CFTree!, CFTree!)

Inserts a new sibling after a given tree.

func CFTreeRemoveAllChildren(CFTree!)

Removes all the children of a tree.

func CFTreeRemove(CFTree!)

Removes a tree from its parent.

func CFTreeSetContext(CFTree!, UnsafePointer&lt;CFTreeContext>!)

Replaces the context of a tree by releasing the old information pointer and retaining the new one.

