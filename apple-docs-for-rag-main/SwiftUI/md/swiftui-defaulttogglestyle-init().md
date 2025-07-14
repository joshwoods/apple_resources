

- SwiftUI
- DefaultToggleStyle
-  init() 

Initializer

# init()

Creates a default toggle style.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init()
```

## Discussion

Don’t call this initializer directly. Instead, use the automatic static variable to create this style:

```
Toggle("Enhance Sound", isOn: $isEnhanced)
    .toggleStyle(.automatic)
```

