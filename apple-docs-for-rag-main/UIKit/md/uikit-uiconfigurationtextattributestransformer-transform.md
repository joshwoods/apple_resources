

- UIKit
- UIConfigurationTextAttributesTransformer
-  transform 

Instance Property

# transform

A closure that defines the text transformation.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
let transform: (AttributeContainer) -> AttributeContainer
```

## Discussion

This closure accepts a container with the current text attributes and returns a container with the new text attributes.

