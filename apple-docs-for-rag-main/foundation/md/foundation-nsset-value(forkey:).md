

- Foundation
- NSSet
-  value(forKey:) 

Instance Method

# value(forKey:)

Return a set containing the results of invoking `valueForKey:` on each of the receiving set’s members.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func value(forKey key: String) -> Any
```

## Parameters 

`key`  

The name of one of the properties of the receiving set’s members.

## Return Value

A set containing the results of invoking `valueForKey:` (with the argument `key`) on each of the receiving set’s members.

## Discussion

The returned set might not have the same number of members as the receiving set. The returned set will not contain any elements corresponding to instances of `valueForKey:` returning `nil` (note that this is in contrast with `NSArray`’s implementation, which may put `NSNull` values in the arrays it returns).

## See Also

### Comparing Sets

func isSubset(of: Set&lt;AnyHashable>) -> Bool

Returns a Boolean value that indicates whether every object in the receiving set is also present in another given set.

func intersects(Set&lt;AnyHashable>) -> Bool

Returns a Boolean value that indicates whether at least one object in the receiving set is also present in another given set.

func isEqual(to: Set&lt;AnyHashable>) -> Bool

Compares the receiving set to another set.

func setValue(Any?, forKey: String)

Invokes `setValue:forKey:` on each of the set’s members.

