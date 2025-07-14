

- SwiftUI
- CheckboxToggleStyle
-  init() 

Initializer

# init()

Creates a checkbox toggle style.

macOS 10.15+

``` source
init()
```

## Discussion

Don’t call this initializer directly. Instead, use the checkbox static variable to create this style:

```
Toggle("Close windows when quitting an app", isOn: $doesClose)
    .toggleStyle(.checkbox)
```

