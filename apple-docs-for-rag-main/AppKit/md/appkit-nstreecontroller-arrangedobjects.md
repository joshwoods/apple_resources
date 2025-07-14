

- AppKit
- NSTreeController
-  arrangedObjects 

Instance Property

# arrangedObjects

The tree controller’s sorted content objects.

macOS

``` source
var arrangedObjects: NSTreeNode { get }
```

## Discussion

The value of this property represents a proxy root tree node containing the tree controller’s sorted content objects. The proxy object responds to children and descendant(at:) messages. This property is observable using key-value observing.

## See Also

### Arranging Objects

func rearrangeObjects()

Use this method to trigger reordering of the tree controller’s content.

