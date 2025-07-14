

- Core Foundation
-  CFTreeInsertSibling(\_:\_:) 

Function

# CFTreeInsertSibling(\_:\_:)

Inserts a new sibling after a given tree.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFTreeInsertSibling(
    _ tree: CFTree!,
    _ newSibling: CFTree!
)
```

## Parameters 

`tree`  

The tree after which to insert `newSibling`. `tree` must have a parent.

`newSibling`  

The sibling to add. `newSibling` must not have a parent.

## Discussion

When a child tree is added to another tree, the child tree is retained by its new parent.

If you want to manipulate an existing tree structure, since `newSibling` must not have a parent you need to remove a tree from its parent in order to move it to a new position. If you do this, you should retain the tree before you actually remove it from its parent (see CFTreeRemove(_:)).

## See Also

### Modifying a Tree

func CFTreeAppendChild(CFTree!, CFTree!)

Adds a new child to a tree as the last in its list of children.

func CFTreeRemoveAllChildren(CFTree!)

Removes all the children of a tree.

func CFTreePrependChild(CFTree!, CFTree!)

Adds a new child to the specified tree as the first in its list of children.

func CFTreeRemove(CFTree!)

Removes a tree from its parent.

func CFTreeSetContext(CFTree!, UnsafePointer&lt;CFTreeContext>!)

Replaces the context of a tree by releasing the old information pointer and retaining the new one.

