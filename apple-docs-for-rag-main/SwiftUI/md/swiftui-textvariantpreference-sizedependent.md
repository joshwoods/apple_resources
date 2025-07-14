

- SwiftUI
- TextVariantPreference
-  sizeDependent 

Type Property

# sizeDependent

The size dependent preference allows the text to take the available space into account when choosing the size variant to display.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static var sizeDependent: SizeDependentTextVariant { get }
```

Available when `Self` is `SizeDependentTextVariant`.

## Discussion

When a Text provides different size options for its content, the size dependent preference chooses the largest option that fits into the available space without truncating or clipping its content.

Note

Only use this option where needed as it incurrs a performance cost on every Text it is applied to, even if the concrete text initializer cannot provide multiple size variants and there is no visual impact.

## Difference to ``doc://com.apple.SwiftUI/documentation/SwiftUI/ViewThatFits``

The sizeDependent text variant preference differs from ViewThatFits both in usage and in behavior. ViewThatFits chooses the first child where the **ideal** size fits the available space. For Text this means that it will only choose texts that can fit their contents into the available space **without a line break**. With this text variant preference, on the other hand, the largest variant is chosen that can fit the available space while respecting all the regular layout rules, such as lineLimit.

To use ViewThatFits, multiple different views have to be provided as the different size options. With this text variant preference, a single Text provides the different size variants intrinsicly. The way it generates these size variants and how many size variants are available depends on the text initializer used.

