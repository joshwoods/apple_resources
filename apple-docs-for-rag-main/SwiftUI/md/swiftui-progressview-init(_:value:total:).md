

- SwiftUI
- ProgressView
-  init(\_:value:total:) 

Initializer

# init(\_:value:total:)

Creates a progress view for showing determinate progress that generates its label from a string.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
nonisolated
init(
    _ title: S,
    value: V?,
    total: V = 1.0
) where Label == Text, CurrentValueLabel == EmptyView, S : StringProtocol, V : BinaryFloatingPoint
```

Available when `Label` conforms to `View` and `CurrentValueLabel` conforms to `View`.

Show all declarations

## Parameters 

`title`  

The string that describes the task in progress.

`value`  

The completed amount of the task to this point, in a range of `0.0` to `total`, or `nil` if the progress is indeterminate.

`total`  

The full amount representing the complete scope of the task, meaning the task is complete if `value` equals `total`. The default value is `1.0`.

## Discussion

If the value is non-`nil`, but outside the range of `0.0` through `total`, the progress view pins the value to those limits, rounding to the nearest possible bound. A value of `nil` represents indeterminate progress, in which case the progress view ignores `total`.

This initializer creates a Text view on your behalf, and treats the title similar to init(verbatim:). See Text for more information about localizing strings. To initialize a determinate progress view with a localized string key, use the corresponding initializer that takes a `LocalizedStringKey` instance.

## See Also

### Creating a determinate progress view

init(Progress)

Creates a progress view for visualizing the given progress instance.

init&lt;V>(value: V?, total: V)

Creates a progress view for showing determinate progress.

init&lt;V>(value: V?, total: V, label: () -> Label)

Creates a progress view for showing determinate progress, with a custom label.

init&lt;V>(value: V?, total: V, label: () -> Label, currentValueLabel: () -> CurrentValueLabel)

Creates a progress view for showing determinate progress, with a custom label.

