

- SwiftUI
- MultiDatePicker
-  init(\_:selection:) 

Initializer

# init(\_:selection:)

Creates an instance that selects multiple dates with an unbounded range.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    selection: Binding>
)
```

Available when `Label` is `Text`.

Show all declarations

## Parameters 

`titleKey`  

The key for the localized title of `self`, describing its purpose.

`selection`  

The date values being displayed and selected.

## See Also

### Picking dates

init(selection: Binding&lt;Set&lt;DateComponents>>, label: () -> Label)

Creates an instance that selects multiple dates with an unbounded range.

