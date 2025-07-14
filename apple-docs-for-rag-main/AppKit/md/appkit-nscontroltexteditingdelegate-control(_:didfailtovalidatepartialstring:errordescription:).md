

- AppKit
- NSControlTextEditingDelegate
-  control(\_:didFailToValidatePartialString:errorDescription:) 

Instance Method

# control(\_:didFailToValidatePartialString:errorDescription:)

Invoked when the formatter for the cell belonging to `control` (or selected cell) rejects a partial string a user is typing into the cell.

macOS

``` source
@MainActor
optional func control(
    _ control: NSControl,
    didFailToValidatePartialString string: String,
    errorDescription error: String?
)
```

## Parameters 

`control`  

The control whose cell rejected the string.

`string`  

The string that includes the character that caused the rejection.

`error`  

A localized, user-presentable string that explains why the string was rejected.

## Discussion

You can implement this method to display a warning message or perform a similar action when the user enters improperly formatted text.

## See Also

### Related Documentation

func isPartialStringValid(String, newEditingString: AutoreleasingUnsafeMutablePointer&lt;NSString?>?, errorDescription: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> Bool

Returns a Boolean value that indicates whether a partial string is valid.

### Validating a Control’s Value

func control(NSControl, isValidObject: Any?) -> Bool

Invoked when the insertion point leaves a cell belonging to the specified control, but before the value of the cell’s object is displayed.

