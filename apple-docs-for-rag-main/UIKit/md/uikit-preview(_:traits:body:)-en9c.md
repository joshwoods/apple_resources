

- UIKit
-  Preview(\_:traits:body:) 

Macro

# Preview(\_:traits:body:)

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS

``` source
@freestanding(declaration)
macro Preview(
    _ name: String? = nil,
    traits: PreviewTrait...,
    @PreviewMacroBodyBuilder body: @escaping @MainActor () -> UIViewController
)
```

## See Also

### Macros

macro Preview(String?, traits: PreviewTrait&lt;Preview.ViewTraits>..., body: () -> UIView)

var UIKIT_HAS_UIFOUNDATION_SYMBOLS: Int32

