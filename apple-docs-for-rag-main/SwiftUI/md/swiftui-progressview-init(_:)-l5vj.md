

- SwiftUI
- ProgressView
-  init(\_:) 

Initializer

# init(\_:)

Creates a progress view for visualizing the given progress instance.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
nonisolated
init(_ progress: Progress) where Label == EmptyView, CurrentValueLabel == EmptyView
```

Available when `Label` conforms to `View` and `CurrentValueLabel` conforms to `View`.

Show all declarations

## Discussion

The progress view synthesizes a default label using the `localizedDescription` of the given progress instance.

## See Also

### Creating a determinate progress view

init&lt;V>(value: V?, total: V)

Creates a progress view for showing determinate progress.

init(_:value:total:)

Creates a progress view for showing determinate progress that generates its label from a string.

init&lt;V>(value: V?, total: V, label: () -> Label)

Creates a progress view for showing determinate progress, with a custom label.

init&lt;V>(value: V?, total: V, label: () -> Label, currentValueLabel: () -> CurrentValueLabel)

Creates a progress view for showing determinate progress, with a custom label.

