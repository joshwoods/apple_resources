

- AppKit
- NSTokenFieldDelegate
-  tokenField(\_:menuForRepresentedObject:) 

Instance Method

# tokenField(\_:menuForRepresentedObject:)

Allows the delegate to provide a menu for the specified represented object.

macOS

``` source
@MainActor
optional func tokenField(
    _ tokenField: NSTokenField,
    menuForRepresentedObject representedObject: Any
) -> NSMenu?
```

## Parameters 

`tokenField`  

The token field that sent the message.

`representedObject`  

A represented object of the token field.

## Return Value

The menu associated with the represented object.

## Discussion

The returned menu should be autoreleased. By default tokens in a token field do not return menus.

## See Also

### Managing Menus for Represented Objects

func tokenField(NSTokenField, hasMenuForRepresentedObject: Any) -> Bool

Allows the delegate to specify whether the given represented object provides a menu.

