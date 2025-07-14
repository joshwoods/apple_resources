

- SwiftUI
- SettingsLink
-  init() 

Initializer

# init()

Creates a settings link with the default system label.

macOS 14.0+

``` source
init() where Label == DefaultSettingsLinkLabel
```

## Discussion

The display of the label may be customized using the `labelStyle(_:)` modifier.

## See Also

### Creating a settings link

init(label: () -> Label)

Creates a settings link with a custom label.

