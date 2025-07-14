

- AVFoundation
- AVVideoOutputSpecification
-  setOutputSettings(\_:for:) 

Instance Method

# setOutputSettings(\_:for:)

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func setOutputSettings(
    _ outputSettings: [String : any Sendable]?,
    for tagCollection: [CMTag]
)
```

## See Also

### Configuring the specification

var defaultOutputSettings: [String : any Sendable]?

var defaultPixelBufferAttributes: [String : Any]?

func setOutputPixelBufferAttributes([String : Any]?, for: [CMTag])

var preferredTagCollections: [[CMTag]]

