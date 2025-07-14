

- AppKit
- NSArrayController
-  arrange(\_:) 

Instance Method

# arrange(\_:)

Returns a given array, appropriately sorted and filtered.

macOS

``` source
func arrange(_ objects: [Any]) -> [Any]
```

## Return Value

An array containing `objects` filtered using the receiver’s filter predicate (see filterPredicate) and sorted according to the receiver’s sortDescriptors.

## Discussion

Subclasses should override this method to use a different sort mechanism, provide custom object arrangement, or (typically only prior to OS X version 10.4, which provides a filter predicate) filter the objects.

## See Also

### Arranging Objects

var arrangedObjects: Any

An array containing the receiver’s content objects arranged using arrange(_:).

func rearrangeObjects()

Triggers filtering of the receiver’s content.

