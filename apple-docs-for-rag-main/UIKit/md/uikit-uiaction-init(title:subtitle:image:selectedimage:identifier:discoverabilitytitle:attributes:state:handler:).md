

- UIKit
- UIAction
-  init(title:subtitle:image:selectedImage:identifier:discoverabilityTitle:attributes:state:handler:) 

Initializer

# init(title:subtitle:image:selectedImage:identifier:discoverabilityTitle:attributes:state:handler:)

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
@MainActor @preconcurrency
convenience init(
    title: String = "",
    subtitle: String? = nil,
    image: UIImage? = nil,
    selectedImage: UIImage? = nil,
    identifier: UIAction.Identifier? = nil,
    discoverabilityTitle: String? = nil,
    attributes: UIMenuElement.Attributes = [],
    state: UIMenuElement.State = .off,
    handler: @escaping UIActionHandler
)
```

