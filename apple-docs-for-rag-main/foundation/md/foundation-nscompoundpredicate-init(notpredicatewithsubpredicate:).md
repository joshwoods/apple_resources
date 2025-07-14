

- Foundation
- NSCompoundPredicate
-  init(notPredicateWithSubpredicate:) 

Initializer

# init(notPredicateWithSubpredicate:)

Returns a new predicate that you form using a NOT operation on a specified predicate.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(notPredicateWithSubpredicate predicate: NSPredicate)
```

## Parameters 

`predicate`  

A predicate.

## Return Value

A new predicate formed by NOT-ing the predicate specified by `predicate`.

## Discussion

For applications linked on macOS 10.5 or later, the `subpredicates` array is copied. For applications linked on OS X v10.4, the `subpredicates` array is retained (for binary compatibility).

## See Also

### Creating Compound Predicates

init(andPredicateWithSubpredicates: [NSPredicate])

Returns a new predicate that you form using an AND operation on the predicates in a specified array.

init(orPredicateWithSubpredicates: [NSPredicate])

Returns a new predicate that you form using an OR operation on the predicates in a specified array.

init(type: NSCompoundPredicate.LogicalType, subpredicates: [NSPredicate])

Returns the receiver that a specified type initializes using predicates from a specified array.

init?(coder: NSCoder)

Creates a predicate by decoding from the coder you specify.

