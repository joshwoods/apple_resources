

- SwiftUI
- ProgressView
-  init(label:) 

Initializer

# init(label:)

Creates a progress view for showing indeterminate progress that displays a custom label.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
nonisolated
init(@ViewBuilder label: () -> Label)
```

Available when `Label` conforms to `View` and `CurrentValueLabel` is `EmptyView`.

## Parameters 

`label`  

A view builder that creates a view that describes the task in progress.

## See Also

### Creating an indeterminate progress view

init()

Creates a progress view for showing indeterminate progress, without a label.

init(LocalizedStringKey)

Creates a progress view for showing indeterminate progress that generates its label from a localized string.

init&lt;S>(S)

Creates a progress view for showing indeterminate progress that generates its label from a string.

