

- AppKit
- NSDocument
-  validateUserInterfaceItem(\_:) 

Instance Method

# validateUserInterfaceItem(\_:)

Validates the specified user interface item that the receiver manages.

macOS

``` source
@MainActor
func validateUserInterfaceItem(_ item: any NSValidatedUserInterfaceItem) -> Bool
```

## Parameters 

`item`  

The user interface item to validate.

## Return Value

true if the item is valid; otherwise, false.

## Discussion

These items currently include only Revert and Save. You can override this method to add more selectors validated by your document subclass.

