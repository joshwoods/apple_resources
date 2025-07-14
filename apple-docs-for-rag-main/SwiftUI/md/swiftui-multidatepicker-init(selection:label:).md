

- SwiftUI
- MultiDatePicker
-  init(selection:label:) 

Initializer

# init(selection:label:)

Creates an instance that selects multiple dates with an unbounded range.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
nonisolated
init(
    selection: Binding>,
    @ViewBuilder label: () -> Label
)
```

Available when `Label` conforms to `View`.

## Parameters 

`selection`  

The date values being displayed and selected.

`label`  

A view that describes the use of the dates.

## See Also

### Picking dates

init(_:selection:)

Creates an instance that selects multiple dates with an unbounded range.

