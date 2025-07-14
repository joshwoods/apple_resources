

- AppKit
- NSTokenFieldDelegate
-  tokenField(\_:hasMenuForRepresentedObject:) 

Instance Method

# tokenField(\_:hasMenuForRepresentedObject:)

Allows the delegate to specify whether the given represented object provides a menu.

macOS

``` source
@MainActor
optional func tokenField(
    _ tokenField: NSTokenField,
    hasMenuForRepresentedObject representedObject: Any
) -> Bool
```

## Parameters 

`tokenField`  

The token field that sent the message.

`representedObject`  

A represented object of the token field.

## Return Value

true if the represented object has a menu, false otherwise.

## Discussion

By default tokens in a token field have no menus.

## See Also

### Managing Menus for Represented Objects

func tokenField(NSTokenField, menuForRepresentedObject: Any) -> NSMenu?

Allows the delegate to provide a menu for the specified represented object.

