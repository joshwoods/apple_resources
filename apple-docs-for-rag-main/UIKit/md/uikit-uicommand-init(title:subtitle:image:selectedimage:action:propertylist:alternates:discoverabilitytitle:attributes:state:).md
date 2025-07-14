

- UIKit
- UICommand
-  init(title:subtitle:image:selectedImage:action:propertyList:alternates:discoverabilityTitle:attributes:state:) 

Initializer

# init(title:subtitle:image:selectedImage:action:propertyList:alternates:discoverabilityTitle:attributes:state:)

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
@MainActor @preconcurrency
convenience init(
    title: String = "",
    subtitle: String? = nil,
    image: UIImage? = nil,
    selectedImage: UIImage? = nil,
    action: Selector,
    propertyList: Any? = nil,
    alternates: [UICommandAlternate] = [],
    discoverabilityTitle: String? = nil,
    attributes: UIMenuElement.Attributes = [],
    state: UIMenuElement.State = .off
)
```

