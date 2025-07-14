

- Foundation
- Formatter
-  isPartialStringValid(\_:newEditingString:errorDescription:) 

Instance Method

# isPartialStringValid(\_:newEditingString:errorDescription:)

Returns a Boolean value that indicates whether a partial string is valid.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isPartialStringValid(
    _ partialString: String,
    newEditingString newString: AutoreleasingUnsafeMutablePointer?,
    errorDescription error: AutoreleasingUnsafeMutablePointer?
) -> Bool
```

## Parameters 

`partialString`  

The text currently in a cell.

`newString`  

If `partialString` needs to be modified, upon return contains the replacement string.

`error`  

If non-`nil`, if validation fails contains an `NSString` object that describes the problem.

## Return Value

true if `partialString` is an acceptable value, otherwise false.

## Discussion

This method is invoked each time the user presses a key while the cell has the keyboard focus—it lets you verify and edit the cell text as the user types it.

In a subclass implementation, evaluate `partialString` according to the context, edit the text if necessary, and return by reference any edited string in `newString`. Return true if `partialString` is acceptable and false if `partialString` is unacceptable. If you return false and `newString` is `nil`, the cell displays `partialString` minus the last character typed. If you return false, you can also return by indirection an `NSString` object (in `error`) that explains the reason why the validation failed; the delegate (if any) of the `NSControl` object managing the cell can then respond to the failure in control:didFailToValidatePartialString:errorDescription:. The selection range will always be set to the end of the text if replacement occurs.

This method is a compatibility method. If a subclass overrides this method and does not override isPartialStringValid(_:proposedSelectedRange:originalString:originalSelectedRange:errorDescription:), this method will be called as before (isPartialStringValid(_:proposedSelectedRange:originalString:originalSelectedRange:errorDescription:) just calls this one by default).

## See Also

### Validating Partial Strings

func isPartialStringValid(AutoreleasingUnsafeMutablePointer&lt;NSString>, proposedSelectedRange: NSRangePointer?, originalString: String, originalSelectedRange: NSRange, errorDescription: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> Bool

This method should be implemented in subclasses that want to validate user changes to a string in a field, where the user changes are not necessarily at the end of the string, and preserve the selection (or set a different one, such as selecting the erroneous part of the string the user has typed).

