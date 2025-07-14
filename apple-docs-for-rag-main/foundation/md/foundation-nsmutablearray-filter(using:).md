

- Foundation
- NSMutableArray
-  filter(using:) 

Instance Method

# filter(using:)

Evaluates a given predicate against the array’s content and leaves only objects that match.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func filter(using predicate: NSPredicate)
```

## Parameters 

`predicate`  

The predicate to evaluate against the array’s elements.

## See Also

### Related Documentation

func filtered(using: NSPredicate) -> [Any]

Evaluates a given predicate against each object in the receiving array and returns a new array containing the objects for which the predicate returns true.

