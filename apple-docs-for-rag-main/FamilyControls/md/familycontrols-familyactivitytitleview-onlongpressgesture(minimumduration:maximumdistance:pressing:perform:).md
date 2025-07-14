

- FamilyControls
- FamilyActivityTitleView
-  onLongPressGesture(minimumDuration:maximumDistance:pressing:perform:) 

Instance Method

# onLongPressGesture(minimumDuration:maximumDistance:pressing:perform:)

Adds an action to perform when this view recognizes a long press gesture.

FamilyControlsSwiftUIiOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedvisionOSwatchOS 6.0–11.4Deprecated

``` source
nonisolated
func onLongPressGesture(
    minimumDuration: Double = 0.5,
    maximumDistance: CGFloat = 10,
    pressing: ((Bool) -> Void)? = nil,
    perform action: @escaping () -> Void
) -> some View
```

