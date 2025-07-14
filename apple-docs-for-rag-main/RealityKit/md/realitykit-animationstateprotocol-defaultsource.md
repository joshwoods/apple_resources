

- RealityKit
- AnimationStateProtocol
-  defaultSource 

Instance Property

# defaultSource

The previous blend stage value.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var defaultSource: Self.ValueType? { get }
```

**Required**

## Discussion

The default source is the value output from the previous blend stage, and initialized with defaultTarget for the first stage.

