

- AppKit
- NSTokenFieldDelegate
-  tokenField(\_:styleForRepresentedObject:) 

Instance Method

# tokenField(\_:styleForRepresentedObject:)

Allows the delegate to return the token style for editing the specified represented object.

macOS

``` source
@MainActor
optional func tokenField(
    _ tokenField: NSTokenField,
    styleForRepresentedObject representedObject: Any
) -> NSTokenField.TokenStyle
```

## Parameters 

`tokenField`  

The token field that sent the message.

`representedObject`  

A represented object of the token field.

## Return Value

The style that should be used to display the representedObject. Possible values are shown in NSTokenStyle Values.

## Discussion

If the delegate implements this method and returns an NSTokenField.TokenStyle that differs from the style set by tokenStyle, the value the delegate returns is preferred.

If the delegate does not implement this method, the token field’s tokenStyle is used.

## See Also

### Displaying Tokenized Strings

func tokenField(NSTokenField, displayStringForRepresentedObject: Any) -> String?

Allows the delegate to provide a string to be displayed as a proxy for the given represented object.

