

- AppKit
- NSTextStorage
-  edited(\_:range:changeInLength:) 

Instance Method

# edited(\_:range:changeInLength:)

Tracks changes made to the text storage object, allowing the text storage to record the full extent of changes.

macOS 10.0+

``` source
func edited(
    _ editedMask: NSTextStorageEditActions,
    range editedRange: NSRange,
    changeInLength delta: Int
)
```

## Parameters 

`editedMask`  

A mask specifying the nature of the changes. You make the value by combining with the C bitwise OR operator the options described in NSTextStorageEditActions.

`editedRange`  

The extent of characters affected before the change took place.

`delta`  

The number of characters added to or removed from `oldRange`. If no characters where edited as noted by `mask`, its value is irrelevant and undefined. For example, when replacing “The” with “Several” in the string “The files couldn’t be saved”, `oldRange` is {0, 3} and `lengthChange` is 4.

## Discussion

This method invokes processEditing() if there are no outstanding beginEditing() calls. `NSTextStorage` invokes this method automatically each time it makes a change to its attributed string. Subclasses that override or add methods that alter their attributed strings directly should invoke this method after making those changes; otherwise you shouldn’t invoke this method. The information accumulated with this method is then used in an invocation of processEditing() to report the affected portion of the receiver.

The methods for querying changes, editedRange and changeInLength, indicate the extent of characters affected after the change. This method expects the characters before the change because that information is readily available as the argument to whatever method performs the change (such as replaceCharacters(in:with:)).

## See Also

### Managing edits

func processEditing()

Cleans up changes to the text storage object and notifies its delegate and layout managers of changes.

