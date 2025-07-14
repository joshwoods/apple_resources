

- ARKit
- ARConfiguration
- ARConfiguration.FrameSemantics
-  init(rawValue:) 

Initializer

# init(rawValue:)

Creates a frame semantics feature.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
init(rawValue: UInt)
```

## Discussion

Initialize an ARConfiguration.FrameSemantics with the value of zero to indicate that no optional frame features are enabled.

You enable a feature by adding it to your configuration’s frameSemantics option set.

