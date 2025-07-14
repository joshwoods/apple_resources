

- AppKit
- NSObjectController
-  validateUserInterfaceItem(\_:) 

Instance Method

# validateUserInterfaceItem(\_:)

Returns whether the receiver can handle the action method for a user interface item.

macOS

``` source
func validateUserInterfaceItem(_ item: any NSValidatedUserInterfaceItem) -> Bool
```

## Parameters 

`item`  

The user interface item to validate. You can send `item` the action and tag messages.

## Return Value

true if the receiver can handle the action method; false if it cannot.

