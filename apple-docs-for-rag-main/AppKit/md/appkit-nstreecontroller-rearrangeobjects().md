

- AppKit
- NSTreeController
-  rearrangeObjects() 

Instance Method

# rearrangeObjects()

Use this method to trigger reordering of the tree controller’s content.

macOS

``` source
func rearrangeObjects()
```

## Discussion

Subclasses should invoke this method if any parameter that affects the arranged objects changes.

## See Also

### Arranging Objects

var arrangedObjects: NSTreeNode

The tree controller’s sorted content objects.

