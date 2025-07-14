

- FamilyControls
- FamilyActivityPicker
-  invalidatableContent(\_:) 

Instance Method

# invalidatableContent(\_:)

Mark the receiver as their content might be invalidated.

FamilyControlsSwiftUIiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
nonisolated
func invalidatableContent(_ invalidatable: Bool = true) -> some View
```

## Parameters 

`invalidatable`  

Whether the receiver content might be invalidated.

## Discussion

Use this modifier to annotate views that display values that are derived from the current state of your data and might be invalidated in response of, for example, user interaction.

The view will change its appearance when `RedactionReasons.invalidated` is present in the environment.

In an interactive widget a view is invalidated from the moment the user interacts with a control on the widget to the moment when a new timeline update has been presented.

