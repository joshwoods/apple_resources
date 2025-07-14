

- Foundation
- NSOrderedSet
-  filtered(using:) 

Instance Method

# filtered(using:)

Evaluates a given predicate against each object in the receiving ordered set and returns a new ordered set containing the objects for which the predicate returns true.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func filtered(using p: NSPredicate) -> NSOrderedSet
```

## Parameters 

`p`  

The predicate against which to evaluate the receiving ordered set’s elements.

## Return Value

A new ordered set containing the objects in the receiving ordered set for which `p` returns true.

## Discussion

For more details, see Predicate Programming Guide.

