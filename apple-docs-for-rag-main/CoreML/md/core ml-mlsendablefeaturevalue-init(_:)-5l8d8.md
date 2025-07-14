

- Core ML
- MLSendableFeatureValue
-  init(\_:) 

Initializer

# init(\_:)

Creates a sendable feature value from a feature value.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init?(_ value: MLFeatureValue)
```

## Discussion

Some feature values are not representable as a sendable values. In those cases this initializer will return `nil`.

