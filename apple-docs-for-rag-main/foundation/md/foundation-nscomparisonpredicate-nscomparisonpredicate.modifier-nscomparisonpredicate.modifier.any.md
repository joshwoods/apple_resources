

- Foundation
- NSComparisonPredicate
- NSComparisonPredicate.Modifier
-  NSComparisonPredicate.Modifier.any 

Case

# NSComparisonPredicate.Modifier.any

A predicate to match with any entry in the destination of a to-many relationship.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case any
```

## Discussion

The left hand side must be a collection. The corresponding predicate compares each value in the left hand side against the right hand side and returns true when it finds the first match—or false if no match is found

## See Also

### Constants

case direct

A predicate to compare directly the left and right hand sides.

case all

A predicate to compare all entries in the destination of a to-many relationship.

case direct

A predicate to compare directly the left and right hand sides.

case all

A predicate to compare all entries in the destination of a to-many relationship.

