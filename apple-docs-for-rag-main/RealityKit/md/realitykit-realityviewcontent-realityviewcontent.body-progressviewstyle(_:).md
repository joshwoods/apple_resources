

- RealityKit
- RealityViewContent
- RealityViewContent.Body
-  progressViewStyle(\_:) 

Instance Method

# progressViewStyle(\_:)

Sets the style for progress views in this view.

RealityKitSwiftUIiOS 14.0+iPadOS 14.0+macOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
nonisolated
func progressViewStyle(_ style: S) -> some View where S : ProgressViewStyle
```

## Parameters 

`style`  

The progress view style to use for this view.

## Discussion

For example, the following code creates a progress view that uses the “circular” style:

```
ProgressView()
    .progressViewStyle(.circular)
```

