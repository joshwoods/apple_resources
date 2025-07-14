

- AppKit
- NSArrayController
-  filterPredicate 

Instance Property

# filterPredicate

A predicate used by the receiver to filter the array controller contents

macOS

``` source
var filterPredicate: NSPredicate? { get set }
```

## Discussion

This property is observable using key-value observing.

## See Also

### Filtering Content

var clearsFilterPredicateOnInsertion: Bool

A Boolean value that indicates whether the receiver automatically clears an existing filter predicate when new items are inserted or added to the content

