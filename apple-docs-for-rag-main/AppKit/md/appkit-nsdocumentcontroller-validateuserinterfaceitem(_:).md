

- AppKit
- NSDocumentController
-  validateUserInterfaceItem(\_:) 

Instance Method

# validateUserInterfaceItem(\_:)

Returns a Boolean value that indicates whether a given user interface item should be enabled.

macOS

``` source
@MainActor
func validateUserInterfaceItem(_ item: any NSValidatedUserInterfaceItem) -> Bool
```

## Parameters 

`item`  

The user interface item to validate. You can send `anItem` the action and tag messages.

## Return Value

true if `item` should be enabled, otherwise false.

## Discussion

Subclasses can override this method to perform additional validations. Subclasses should call the underlying method on `super` in their implementation for items they don’t handle themselves.

