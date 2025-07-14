

- FamilyControls
- FamilyActivityIconView
-  navigationBarHidden(\_:) 

Instance Method

# navigationBarHidden(\_:)

Hides the navigation bar for this view.

FamilyControlsSwiftUIiOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedtvOS 13.0+visionOS 1.0+watchOS 6.0–11.4Deprecated

``` source
nonisolated
func navigationBarHidden(_ hidden: Bool) -> some View
```

## Parameters 

`hidden`  

A Boolean value that indicates whether to hide the navigation bar.

## Discussion

Use `navigationBarHidden(_:)` to hide the navigation bar. This modifier only takes effect when this view is inside of and visible within a `NavigationView`.

