

- FamilyControls
- FamilyActivityIconView
-  accessibility(selectionIdentifier:) 

Instance Method

# accessibility(selectionIdentifier:)

Sets a selection identifier for this view’s accessibility element.

FamilyControlsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0–1.0DeprecatedwatchOS 6.0+

``` source
nonisolated
func accessibility(selectionIdentifier: AnyHashable) -> ModifiedContent
```

## Discussion

Picker uses the value to determine what node to use for the accessibility value.

