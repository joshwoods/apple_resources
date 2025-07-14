

- Foundation
- Formatter
-  isPartialStringValid(\_:proposedSelectedRange:originalString:originalSelectedRange:errorDescription:) 

Instance Method

# isPartialStringValid(\_:proposedSelectedRange:originalString:originalSelectedRange:errorDescription:)

This method should be implemented in subclasses that want to validate user changes to a string in a field, where the user changes are not necessarily at the end of the string, and preserve the selection (or set a different one, such as selecting the erroneous part of the string the user has typed).

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isPartialStringValid(
    _ partialStringPtr: AutoreleasingUnsafeMutablePointer,
    proposedSelectedRange proposedSelRangePtr: NSRangePointer?,
    originalString origString: String,
    originalSelectedRange origSelRange: NSRange,
    errorDescription error: AutoreleasingUnsafeMutablePointer?
) -> Bool
```

## Parameters 

`partialStringPtr`  

The new string to validate.

`proposedSelRangePtr`  

The selection range that will be used if the string is accepted or replaced.

`origString`  

The original string, before the proposed change.

`origSelRange`  

The selection range over which the change is to take place.

If the user change is a deletion, `origSelRange` contains the range of the deleted characters.

`error`  

If non-`nil`, if validation fails contains an `NSString` object that describes the problem.

## Return Value

true if `partialStringPtr` is acceptable, otherwise false.

## Discussion

In a subclass implementation, evaluate `partialString` according to the context. Return true if `partialStringPtr` is acceptable and false if `partialStringPtr` is unacceptable. If you return false and assign a new string to `partialStringPtr` and a new range to `proposedSelRangePtr`, the string and selection range are changed, otherwise, if no values are assigned to `partialStringPtr` or `proposedSelRangePtr`, the change is rejected. If you return false, you can also return by indirection an `NSString` object (in `error`) that explains the reason why the validation failed; the delegate (if any) of the `NSControl` object managing the cell can then respond to the failure in control:didFailToValidatePartialString:errorDescription:.

## See Also

### Validating Partial Strings

func isPartialStringValid(String, newEditingString: AutoreleasingUnsafeMutablePointer&lt;NSString?>?, errorDescription: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> Bool

Returns a Boolean value that indicates whether a partial string is valid.

