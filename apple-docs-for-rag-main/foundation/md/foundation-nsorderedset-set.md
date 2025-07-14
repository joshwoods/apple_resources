

- Foundation
- NSOrderedSet
-  set 

Instance Property

# set

A representation of the set containing the contents of the ordered set.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var set: Set { get }
```

## Discussion

This returns a proxy object for the receiving ordered set, which acts like an immutable set.

While you cannot mutate the ordered set through this proxy, mutations to the original ordered set will be reflected in the proxy and it will appear to change spontaneously, because a copy of the ordered set is not being made.

## See Also

### Converting Other Collections

var array: [Any]

A representation of the ordered set as an array.

