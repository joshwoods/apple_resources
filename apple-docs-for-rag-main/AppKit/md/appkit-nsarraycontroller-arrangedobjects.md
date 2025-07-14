

- AppKit
- NSArrayController
-  arrangedObjects 

Instance Property

# arrangedObjects

An array containing the receiver’s content objects arranged using arrange(_:).

macOS

``` source
var arrangedObjects: Any { get }
```

## Discussion

This property is observable using key-value observing.

## See Also

### Arranging Objects

func arrange([Any]) -> [Any]

Returns a given array, appropriately sorted and filtered.

func rearrangeObjects()

Triggers filtering of the receiver’s content.

