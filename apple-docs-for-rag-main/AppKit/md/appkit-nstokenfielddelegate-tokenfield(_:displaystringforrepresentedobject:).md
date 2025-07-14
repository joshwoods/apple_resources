

- AppKit
- NSTokenFieldDelegate
-  tokenField(\_:displayStringForRepresentedObject:) 

Instance Method

# tokenField(\_:displayStringForRepresentedObject:)

Allows the delegate to provide a string to be displayed as a proxy for the given represented object.

macOS

``` source
@MainActor
optional func tokenField(
    _ tokenField: NSTokenField,
    displayStringForRepresentedObject representedObject: Any
) -> String?
```

## Parameters 

`tokenField`  

The token field that sent the message.

`representedObject`  

A represented object of the token field.

## Return Value

The string to be used as a proxy for `representedObject`. If you return `nil` or do not implement this method, then `representedObject` is displayed as the string.

## See Also

### Related Documentation

Token Field Programming Guide

### Displaying Tokenized Strings

func tokenField(NSTokenField, styleForRepresentedObject: Any) -> NSTokenField.TokenStyle

Allows the delegate to return the token style for editing the specified represented object.

