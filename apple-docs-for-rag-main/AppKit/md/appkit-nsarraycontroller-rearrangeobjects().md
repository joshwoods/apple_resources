

- AppKit
- NSArrayController
-  rearrangeObjects() 

Instance Method

# rearrangeObjects()

Triggers filtering of the receiver’s content.

macOS

``` source
func rearrangeObjects()
```

## Discussion

This method invokes arrange(_:).

When you detect that filtering criteria change (such as when listening to the text sent by an `NSSearchField` instance), invoke this method on `self`.

## See Also

### Related Documentation

func didChangeArrangementCriteria()

Invoked when any criteria for arranging objects change.

### Arranging Objects

func arrange([Any]) -> [Any]

Returns a given array, appropriately sorted and filtered.

var arrangedObjects: Any

An array containing the receiver’s content objects arranged using arrange(_:).

