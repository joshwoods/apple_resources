

- Assignables
- AssignedWorkDocumentView
-  scrollIndicators(\_:axes:) 

Instance Method

# scrollIndicators(\_:axes:)

Sets the visibility of scroll indicators within this view.

AssignablesSwiftUIiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
nonisolated
func scrollIndicators(
    _ visibility: ScrollIndicatorVisibility,
    axes: Axis.Set = [.vertical, .horizontal]
) -> some View
```

## Parameters 

`visibility`  

The visibility to apply to scrollable views.

`axes`  

The axes of scrollable views that the visibility applies to.

## Return Value

A view with the specified scroll indicator visibility.

## Discussion

Use this modifier to hide or show scroll indicators on scrollable content in views like a `ScrollView`, `List`, or `TextEditor`. This modifier applies the prefered visibility to any scrollable content within a view hierarchy.

```
ScrollView {
    VStack(alignment: .leading) {
        ForEach(0..

Use the `ScrollIndicatorVisibility/hidden` value to indicate that you prefer that views never show scroll indicators along a given axis. Use `ScrollIndicatorVisibility/visible` when you prefer that views show scroll indicators. Depending on platform conventions, visible scroll indicators might only appear while scrolling. Pass `ScrollIndicatorVisibility/automatic` to allow views to decide whether or not to show their indicators.

