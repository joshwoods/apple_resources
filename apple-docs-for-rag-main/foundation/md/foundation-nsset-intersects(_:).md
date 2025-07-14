

- Foundation
- NSSet
-  intersects(\_:) 

Instance Method

# intersects(\_:)

Returns a Boolean value that indicates whether at least one object in the receiving set is also present in another given set.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func intersects(_ otherSet: Set) -> Bool
```

## Parameters 

`otherSet`  

The set with which to compare the receiving set.

## Return Value

true if at least one object in the receiving set is also present in `otherSet`, otherwise false.

## Discussion

Object equality is tested using isEqual:.

## See Also

### Comparing Sets

func isSubset(of: Set&lt;AnyHashable>) -> Bool

Returns a Boolean value that indicates whether every object in the receiving set is also present in another given set.

func isEqual(to: Set&lt;AnyHashable>) -> Bool

Compares the receiving set to another set.

func value(forKey: String) -> Any

Return a set containing the results of invoking `valueForKey:` on each of the receiving set’s members.

func setValue(Any?, forKey: String)

Invokes `setValue:forKey:` on each of the set’s members.

