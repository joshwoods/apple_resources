

- Foundation
- NSPredicate
-  predicateFormat 

Instance Property

# predicateFormat

The predicate’s format string.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var predicateFormat: String { get }
```

## Discussion

The return value of this property is not guaranteed to be the same as the string used to create the predicate using predicateWithFormat: or similar methods.

You cannot use this method to create a persistent representation of a predicate suitable for recreating the original predicate. If you need a persistent representation of a predicate, create an archive instead, as described in Object archiving (NSPredicate adopts the NSCoding protocol).

