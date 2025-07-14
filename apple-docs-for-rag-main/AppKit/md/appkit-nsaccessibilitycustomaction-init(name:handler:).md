

- AppKit
- NSAccessibilityCustomAction
-  init(name:handler:) 

Initializer

# init(name:handler:)

Creates a custom action object with the specified name and handler.

macOS 10.13+

``` source
init(
    name: String,
    handler: (() -> Bool)? = nil
)
```

## See Also

### Creating a Custom Action

init(name: String, target: any NSObjectProtocol, selector: Selector)

Creates a custom action object with the specified name, target, and selector.

