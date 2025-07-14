

- SwiftUI
- ButtonToggleStyle
-  init() 

Initializer

# init()

Creates a button toggle style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+watchOS 9.0+

``` source
init()
```

## Discussion

Don’t call this initializer directly. Instead, use the button static variable to create this style:

```
Toggle(isOn: $isFlagged) {
    Label("Flag", systemImage: "flag.fill")
}
.toggleStyle(.button)
```

