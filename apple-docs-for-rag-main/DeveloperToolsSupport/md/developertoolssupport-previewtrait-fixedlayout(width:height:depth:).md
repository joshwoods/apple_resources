

- DeveloperToolsSupport
- PreviewTrait
-  fixedLayout(width:height:depth:) 

Type Method

# fixedLayout(width:height:depth:)

Centers the preview in a fixed-size, 3D container.

visionOS 1.0+

``` source
@MainActor
static func fixedLayout(
    width: CGFloat,
    height: CGFloat,
    depth: CGFloat
) -> PreviewTrait
```

Available when `T` is `Preview.ViewTraits`.

## Discussion

This is the same as PreviewLayout.fixed3D(width:height:depth:).

