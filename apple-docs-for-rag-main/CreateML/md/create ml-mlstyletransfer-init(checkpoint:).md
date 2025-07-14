

- Create ML
- MLStyleTransfer
-  init(checkpoint:) 

Initializer

# init(checkpoint:)

Creates a style transfer model from a training session checkpoint.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
init(checkpoint: MLCheckpoint) throws
```

## Parameters 

`checkpoint`  

A checkpoint from a style transfer training session.

## Discussion

You can only use a checkpoint from a style transfer model’s training session if its phase property is MLPhase.training.

