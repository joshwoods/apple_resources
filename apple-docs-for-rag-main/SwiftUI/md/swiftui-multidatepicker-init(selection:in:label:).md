

- SwiftUI
- MultiDatePicker
-  init(selection:in:label:) 

Initializer

# init(selection:in:label:)

Creates an instance that selects multiple dates on or after some start date.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
nonisolated
init(
    selection: Binding>,
    in bounds: PartialRangeFrom,
    @ViewBuilder label: () -> Label
)
```

Available when `Label` conforms to `View`.

Show all declarations

## Parameters 

`selection`  

The date values being displayed and selected.

`bounds`  

The open range from some selectable start date.

`label`  

A view that describes the use of the dates.

## See Also

### Picking dates in a range

init(_:selection:in:)

Creates an instance that selects multiple dates on or after some start date.

