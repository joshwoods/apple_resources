

- AppKit
- NSArrayController
-  clearsFilterPredicateOnInsertion 

Instance Property

# clearsFilterPredicateOnInsertion

A Boolean value that indicates whether the receiver automatically clears an existing filter predicate when new items are inserted or added to the content

macOS

``` source
var clearsFilterPredicateOnInsertion: Bool { get set }
```

## Discussion

The default is true. This property is observable using key-value observing.

## See Also

### Filtering Content

var filterPredicate: NSPredicate?

A predicate used by the receiver to filter the array controller contents

