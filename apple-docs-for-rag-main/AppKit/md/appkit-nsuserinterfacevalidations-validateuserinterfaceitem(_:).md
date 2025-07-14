

- AppKit
- NSUserInterfaceValidations
-  validateUserInterfaceItem(\_:) 

Instance Method

# validateUserInterfaceItem(\_:)

Returns a Boolean value that indicates whether the sender should be enabled.

macOS

``` source
@MainActor
func validateUserInterfaceItem(_ item: any NSValidatedUserInterfaceItem) -> Bool
```

**Required**

## Parameters 

`item`  

The user interface item to validate. You can send `anItem` the action and tag messages.

## Return Value

true if the user interface item should be enabled, otherwise false.

## See Also

### Related Documentation

User Interface Validation

