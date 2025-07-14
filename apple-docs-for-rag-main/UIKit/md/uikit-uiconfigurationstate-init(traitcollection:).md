

- UIKit
- UIConfigurationState
-  init(traitCollection:) 

Initializer

# init(traitCollection:)

Creates a view configuration state with the specified trait collection.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
init(traitCollection: UITraitCollection)
```

**Required**

## Discussion

Typically, you don’t create a configuration state yourself. To obtain a configuration state, override the updateConfiguration(using:) method in your view subclass and use the state parameter. Outside of this method, you can get a view’s configuration state by using its configurationState property.

