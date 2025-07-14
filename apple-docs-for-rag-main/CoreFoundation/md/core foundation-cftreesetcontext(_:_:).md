

- Core Foundation
-  CFTreeSetContext(\_:\_:) 

Function

# CFTreeSetContext(\_:\_:)

Replaces the context of a tree by releasing the old information pointer and retaining the new one.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFTreeSetContext(
    _ tree: CFTree!,
    _ context: UnsafePointer!
)
```

## Parameters 

`tree`  

The tree to modify.

`context`  

The CFTreeContext structure to be copied and used as the context of the new tree. The information pointer will be retained by the tree if a retain function is provided. If this value is not a valid C pointer to a CFTreeContext structure-sized block of storage, the result is undefined. If the version number of the storage is not a valid CFTreeContext version number, the result is undefined.

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

func CFTreeRemove(CFTree!)

Removes a tree from its parent.

