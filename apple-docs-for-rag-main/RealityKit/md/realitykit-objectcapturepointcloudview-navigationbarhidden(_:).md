

- RealityKit
- ObjectCapturePointCloudView
-  navigationBarHidden(\_:) 

Instance Method

# navigationBarHidden(\_:)

Hides the navigation bar for this view.

RealityKitSwiftUIiOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedtvOS 13.0+visionOS 1.0–2.4DeprecatedwatchOS 6.0+

``` source
nonisolated
func navigationBarHidden(_ hidden: Bool) -> some View
```

## Parameters 

`hidden`  

A Boolean value that indicates whether to hide the navigation bar.

## Discussion

Use `navigationBarHidden(_:)` to hide the navigation bar. This modifier only takes effect when this view is inside of and visible within a `NavigationView`.

