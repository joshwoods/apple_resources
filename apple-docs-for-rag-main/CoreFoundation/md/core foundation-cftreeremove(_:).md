

- Core Foundation
-  CFTreeRemove(\_:) 

Function

# CFTreeRemove(\_:)

Removes a tree from its parent.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFTreeRemove(_ tree: CFTree!)
```

## Parameters 

`tree`  

The tree to remove from its parent.

## Discussion

When a child tree is removed from its parent, the parent releases it. If you want to use the child after you have removed it, you should ensure you retain it before removing it from its parent.

## See Also

### Modifying a Tree

func CFTreeAppendChild(CFTree!, CFTree!)

Adds a new child to a tree as the last in its list of children.

func CFTreeInsertSibling(CFTree!, CFTree!)

Inserts a new sibling after a given tree.

func CFTreeRemoveAllChildren(CFTree!)

Removes all the children of a tree.

func CFTreePrependChild(CFTree!, CFTree!)

Adds a new child to the specified tree as the first in its list of children.

func CFTreeSetContext(CFTree!, UnsafePointer&lt;CFTreeContext>!)

Replaces the context of a tree by releasing the old information pointer and retaining the new one.

