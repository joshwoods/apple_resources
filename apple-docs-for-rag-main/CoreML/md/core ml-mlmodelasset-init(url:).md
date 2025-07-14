

- Core ML
- MLModelAsset
-  init(url:) 

Initializer

# init(url:)

Constructs a ModelAsset from a compiled model URL.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
convenience init(url compiledModelURL: URL) throws
```

## Parameters 

`compiledModelURL`  

Location on the disk where the model asset is present.

## Return Value

A model asset or nil if there is an error.

