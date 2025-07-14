

- Assignables
- AssignableDocumentView
-  navigationBarHidden(\_:) 

Instance Method

# navigationBarHidden(\_:)

Hides the navigation bar for this view.

AssignablesSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func navigationBarHidden(_ hidden: Bool) -> some View
```

## Parameters 

`hidden`  

A Boolean value that indicates whether to hide the navigation bar.

## Discussion

Use `navigationBarHidden(_:)` to hide the navigation bar. This modifier only takes effect when this view is inside of and visible within a `NavigationView`.

