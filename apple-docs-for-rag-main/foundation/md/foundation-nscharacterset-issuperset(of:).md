

- Foundation
- NSCharacterSet
-  isSuperset(of:) 

Instance Method

# isSuperset(of:)

Returns a Boolean value that indicates whether the receiver is a superset of another given character set.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isSuperset(of theOtherSet: CharacterSet) -> Bool
```

## Parameters 

`theOtherSet`  

A character set.

## Return Value

true if the receiver is a superset of `theOtherSet`, otherwise false.

## See Also

### Testing Set Membership

func characterIsMember(unichar) -> Bool

Returns a Boolean value that indicates whether a given character is in the receiver.

func hasMemberInPlane(UInt8) -> Bool

Returns a Boolean value that indicates whether the receiver has at least one member in a given character plane.

func longCharacterIsMember(UTF32Char) -> Bool

Returns a Boolean value that indicates whether a given long character is a member of the receiver.

