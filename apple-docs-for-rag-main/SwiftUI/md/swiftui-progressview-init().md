

- SwiftUI
- ProgressView
-  init() 

Initializer

# init()

Creates a progress view for showing indeterminate progress, without a label.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
nonisolated
init() where Label == EmptyView
```

Available when `Label` conforms to `View` and `CurrentValueLabel` is `EmptyView`.

## See Also

### Creating an indeterminate progress view

init(label: () -> Label)

Creates a progress view for showing indeterminate progress that displays a custom label.

init(LocalizedStringKey)

Creates a progress view for showing indeterminate progress that generates its label from a localized string.

init&lt;S>(S)

Creates a progress view for showing indeterminate progress that generates its label from a string.

