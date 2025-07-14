

- MusicKit
- ArtworkImage
-  navigationBarHidden(\_:) Deprecated

Instance Method

# navigationBarHidden(\_:)

Hides the navigation bar for this view.

MusicKitSwiftUIiOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedtvOS 13.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 6.0–11.4Deprecated

``` source
nonisolated
func navigationBarHidden(_ hidden: Bool) -> some View
```

Deprecated

Use toolbar(.hidden)

## Parameters 

`hidden`  

A Boolean value that indicates whether to hide the navigation bar.

## Discussion

Use `navigationBarHidden(_:)` to hide the navigation bar. This modifier only takes effect when this view is inside of and visible within a `NavigationView`.

