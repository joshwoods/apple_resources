

- RealityKit
- RealityViewContent
- RealityViewContent.Body
-  accessibility(sortPriority:) 

Instance Method

# accessibility(sortPriority:)

Sets the sort priority order for this view’s accessibility element, relative to other elements at the same level.

RealityKitSwiftUIiOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0+visionOS 1.0–2.4DeprecatedwatchOS 6.0+

``` source
nonisolated
func accessibility(sortPriority: Double) -> ModifiedContent
```

## Discussion

Higher numbers are sorted first. The default sort priority is zero.

