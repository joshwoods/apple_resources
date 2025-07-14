

- Foundation
- NSCharacterSet
-  hasMemberInPlane(\_:) 

Instance Method

# hasMemberInPlane(\_:)

Returns a Boolean value that indicates whether the receiver has at least one member in a given character plane.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func hasMemberInPlane(_ thePlane: UInt8) -> Bool
```

## Parameters 

`thePlane`  

A character plane.

## Return Value

true if the receiver has at least one member in `thePlane`, otherwise false.

## Discussion

This method makes it easier to find the plane containing the members of the current character set. The Basic Multilingual Plane (BMP) is plane `0`.

## See Also

### Testing Set Membership

func characterIsMember(unichar) -> Bool

Returns a Boolean value that indicates whether a given character is in the receiver.

func isSuperset(of: CharacterSet) -> Bool

Returns a Boolean value that indicates whether the receiver is a superset of another given character set.

func longCharacterIsMember(UTF32Char) -> Bool

Returns a Boolean value that indicates whether a given long character is a member of the receiver.

