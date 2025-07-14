

- AppKit
- NSControlTextEditingDelegate
-  control(\_:isValidObject:) 

Instance Method

# control(\_:isValidObject:)

Invoked when the insertion point leaves a cell belonging to the specified control, but before the value of the cell’s object is displayed.

macOS

``` source
@MainActor
optional func control(
    _ control: NSControl,
    isValidObject obj: Any?
) -> Bool
```

## Parameters 

`control`  

The control whose object value needs to be validated.

`obj`  

The object value to validate.

## Return Value

true if you want to allow the control to display the specified value; otherwise, false to reject the value and return the cursor to the control’s cell.

## Discussion

This method gives the delegate the opportunity to validate the contents of the control’s cell (or selected cell). In validating, the delegate should check the value in the `object` parameter and determine if it falls within a permissible range, has required attributes, accords with a given context, and so on. Examples of objects subject to such evaluations are an `NSDate` object that should not represent a future date or a monetary amount (represented by an `NSNumber` object) that exceeds a predetermined limit.

## See Also

### Related Documentation

Control and Cell Programming Topics

### Validating a Control’s Value

func control(NSControl, didFailToValidatePartialString: String, errorDescription: String?)

Invoked when the formatter for the cell belonging to `control` (or selected cell) rejects a partial string a user is typing into the cell.

