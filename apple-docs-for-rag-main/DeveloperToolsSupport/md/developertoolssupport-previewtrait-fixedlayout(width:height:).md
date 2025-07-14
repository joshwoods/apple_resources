

- DeveloperToolsSupport
- PreviewTrait
-  fixedLayout(width:height:) 

Type Method

# fixedLayout(width:height:)

Center the preview in a fixed size container with the given dimensions.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@MainActor
static func fixedLayout(
    width: CGFloat,
    height: CGFloat
) -> PreviewTrait
```

Available when `T` is `Preview.ViewTraits`.

## Discussion

This is the same as PreviewLayout.fixed(width:height:).

