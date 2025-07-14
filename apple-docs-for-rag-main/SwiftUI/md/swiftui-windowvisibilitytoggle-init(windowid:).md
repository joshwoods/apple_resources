

- SwiftUI
- WindowVisibilityToggle
-  init(windowID:) 

Initializer

# init(windowID:)

Create a window visibility toggle to alter the visibility of a specific window.

macOS 15.0+

``` source
init(windowID: String) where Label == DefaultWindowVisibilityToggleLabel
```

## Parameters 

`windowID`  

The `id` of the singleton window type that should be toggled. If this is not a valid id, the toggle will be disabled and non-functional.

