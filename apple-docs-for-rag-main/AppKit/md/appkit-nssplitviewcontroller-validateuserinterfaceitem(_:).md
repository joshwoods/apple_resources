

- AppKit
- NSSplitViewController
-  validateUserInterfaceItem(\_:) 

Instance Method

# validateUserInterfaceItem(\_:)

Returns a Boolean value that indicates whether to enable the specified item.

macOS 10.11+

``` source
@MainActor
func validateUserInterfaceItem(_ item: any NSValidatedUserInterfaceItem) -> Bool
```

## Parameters 

`item`  

The user interface item to validate.

## Return Value

true if the specified item responds to toggleSidebar(_:), false if it doesn’t.

