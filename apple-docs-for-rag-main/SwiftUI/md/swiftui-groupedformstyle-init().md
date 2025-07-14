

- SwiftUI
- GroupedFormStyle
-  init() 

Initializer

# init()

Creates a form style with scrolling, grouped rows.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init()
```

## Discussion

Don’t call this initializer directly. Instead, use the grouped static variable to create this style:

```
Form {
   ...
}
.formStyle(.grouped)
```

