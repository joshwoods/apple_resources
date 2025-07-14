

- AppKit
- NSArrayController
-  canInsert 

Instance Property

# canInsert

Returns a Boolean value that indicates whether an object can be inserted into the receiver’s content collection.

macOS

``` source
var canInsert: Bool { get }
```

## Return Value

true if an object can be inserted into the receiver’s content collection, otherwise false.

## Discussion

The result of this method can be used by a binding to enable user interface items.

This property is observable using key-value observing.

## See Also

### Inserting

func insert(Any?)

Creates a new object and inserts it into the receiver’s content array.

