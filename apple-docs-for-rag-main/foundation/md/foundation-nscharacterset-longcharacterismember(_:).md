

- Foundation
- NSCharacterSet
-  longCharacterIsMember(\_:) 

Instance Method

# longCharacterIsMember(\_:)

Returns a Boolean value that indicates whether a given long character is a member of the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func longCharacterIsMember(_ theLongChar: UTF32Char) -> Bool
```

## Parameters 

`theLongChar`  

A UTF32 character.

## Return Value

true if `theLongChar` is in the receiver, otherwise false.

## Discussion

This method supports the specification of 32-bit characters.

## See Also

### Testing Set Membership

func characterIsMember(unichar) -> Bool

Returns a Boolean value that indicates whether a given character is in the receiver.

func hasMemberInPlane(UInt8) -> Bool

Returns a Boolean value that indicates whether the receiver has at least one member in a given character plane.

func isSuperset(of: CharacterSet) -> Bool

Returns a Boolean value that indicates whether the receiver is a superset of another given character set.

