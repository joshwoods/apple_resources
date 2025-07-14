

- AppKit
- NSControlTextEditingDelegate
-  control(\_:didFailToFormatString:errorDescription:) 

Instance Method

# control(\_:didFailToFormatString:errorDescription:)

Invoked when the formatter for the cell belonging to the specified control cannot convert a string to an underlying object.

macOS

``` source
@MainActor
optional func control(
    _ control: NSControl,
    didFailToFormatString string: String,
    errorDescription error: String?
) -> Bool
```

## Parameters 

`control`  

The control whose cell could not convert the string.

`string`  

The string that could not be converted.

`error`  

A localized, user-presentable string that explains why the conversion failed.

## Return Value

true if the value in the string parameter should be accepted as is; otherwise, false if the value in the parameter should be rejected.

## Discussion

Your implementation of this method should evaluate the error or query the user an appropriate value indicating whether the string should be accepted or rejected.

## See Also

### Related Documentation

func getObjectValue(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>?, for: String, errorDescription: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> Bool

The default implementation of this method raises an exception.

