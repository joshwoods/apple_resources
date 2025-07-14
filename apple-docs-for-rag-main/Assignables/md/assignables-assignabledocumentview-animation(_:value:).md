

- Assignables
- AssignableDocumentView
-  animation(\_:value:) 

Instance Method

# animation(\_:value:)

Applies the given animation to this view when the specified value changes.

AssignablesSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
nonisolated
func animation(
    _ animation: Animation?,
    value: V
) -> some View where V : Equatable
```

## Parameters 

`animation`  

The animation to apply. If `animation` is `nil`, the view doesn’t animate.

`value`  

A value to monitor for changes.

## Return Value

A view that applies `animation` to this view whenever `value` changes.

