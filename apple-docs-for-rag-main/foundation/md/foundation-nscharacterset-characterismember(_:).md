

- Foundation
- NSCharacterSet
-  characterIsMember(\_:) 

Instance Method

# characterIsMember(\_:)

Returns a Boolean value that indicates whether a given character is in the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func characterIsMember(_ aCharacter: unichar) -> Bool
```

## Parameters 

`aCharacter`  

The character to test for membership of the receiver.

## Return Value

true if `aCharacter` is in the receiving character set, otherwise false.

## See Also

### Testing Set Membership

func hasMemberInPlane(UInt8) -> Bool

Returns a Boolean value that indicates whether the receiver has at least one member in a given character plane.

func isSuperset(of: CharacterSet) -> Bool

Returns a Boolean value that indicates whether the receiver is a superset of another given character set.

func longCharacterIsMember(UTF32Char) -> Bool

Returns a Boolean value that indicates whether a given long character is a member of the receiver.

