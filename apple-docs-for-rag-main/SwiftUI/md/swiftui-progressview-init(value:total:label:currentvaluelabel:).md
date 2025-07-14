

- SwiftUI
- ProgressView
-  init(value:total:label:currentValueLabel:) 

Initializer

# init(value:total:label:currentValueLabel:)

Creates a progress view for showing determinate progress, with a custom label.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
nonisolated
init(
    value: V?,
    total: V = 1.0,
    @ViewBuilder label: () -> Label,
    @ViewBuilder currentValueLabel: () -> CurrentValueLabel
) where V : BinaryFloatingPoint
```

Available when `Label` conforms to `View` and `CurrentValueLabel` conforms to `View`.

## Parameters 

`value`  

The completed amount of the task to this point, in a range of `0.0` to `total`, or `nil` if the progress is indeterminate.

`total`  

The full amount representing the complete scope of the task, meaning the task is complete if `value` equals `total`. The default value is `1.0`.

`label`  

A view builder that creates a view that describes the task in progress.

`currentValueLabel`  

A view builder that creates a view that describes the level of completed progress of the task.

## Discussion

If the value is non-`nil`, but outside the range of `0.0` through `total`, the progress view pins the value to those limits, rounding to the nearest possible bound. A value of `nil` represents indeterminate progress, in which case the progress view ignores `total`.

## See Also

### Creating a determinate progress view

init(Progress)

Creates a progress view for visualizing the given progress instance.

init&lt;V>(value: V?, total: V)

Creates a progress view for showing determinate progress.

init(_:value:total:)

Creates a progress view for showing determinate progress that generates its label from a string.

init&lt;V>(value: V?, total: V, label: () -> Label)

Creates a progress view for showing determinate progress, with a custom label.

