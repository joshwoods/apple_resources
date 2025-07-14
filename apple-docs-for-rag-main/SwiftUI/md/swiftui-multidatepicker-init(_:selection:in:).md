

- SwiftUI
- MultiDatePicker
-  init(\_:selection:in:) 

Initializer

# init(\_:selection:in:)

Creates an instance that selects multiple dates on or after some start date.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    selection: Binding>,
    in bounds: PartialRangeFrom
)
```

Available when `Label` is `Text`.

Show all declarations

## Parameters 

`titleKey`  

The key for the localized title of `self`, describing its purpose.

`selection`  

The date values being displayed and selected.

`bounds`  

The open range from some selectable start date.

## See Also

### Picking dates in a range

init(selection:in:label:)

Creates an instance that selects multiple dates on or after some start date.

