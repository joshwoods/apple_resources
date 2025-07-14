

- Foundation
- CharacterSet
-  hasMember(inPlane:) 

Instance Method

# hasMember(inPlane:)

Returns true if the `CharacterSet` has a member in the specified plane.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func hasMember(inPlane plane: UInt8) -> Bool
```

## Discussion

This method makes it easier to find the plane containing the members of the current character set. The Basic Multilingual Plane (BMP) is plane 0.

## See Also

### Combining Character Sets

func formIntersection(CharacterSet)

Sets the value to an intersection of the `CharacterSet` with another `CharacterSet`.

func formSymmetricDifference(CharacterSet)

Sets the value to an exclusive or of the `CharacterSet` with another `CharacterSet`.

func formUnion(CharacterSet)

Sets the value to a union of the `CharacterSet` with another `CharacterSet`.

func insert(charactersIn: String)

Insert the values from the specified string into the `CharacterSet`.

func intersection(CharacterSet) -> CharacterSet

Returns an intersection of the `CharacterSet` with another `CharacterSet`.

func invert()

Invert the contents of the `CharacterSet`.

func isSuperset(of: CharacterSet) -> Bool

Returns true if `self` is a superset of `other`.

func remove(charactersIn: String)

Remove the values from the specified string from the `CharacterSet`.

func subtracting(CharacterSet) -> CharacterSet

Returns a `CharacterSet` created by removing elements in `other` from `self`.

func symmetricDifference(CharacterSet) -> CharacterSet

Returns an exclusive or of the `CharacterSet` with another `CharacterSet`.

func union(CharacterSet) -> CharacterSet

Returns a union of the `CharacterSet` with another `CharacterSet`.

