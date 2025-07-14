

- AppKit
- NSAccessibilityCustomAction
-  init(name:target:selector:) 

Initializer

# init(name:target:selector:)

Creates a custom action object with the specified name, target, and selector.

macOS 10.13+

``` source
init(
    name: String,
    target: any NSObjectProtocol,
    selector: Selector
)
```

## See Also

### Creating a Custom Action

init(name: String, handler: (() -> Bool)?)

Creates a custom action object with the specified name and handler.

