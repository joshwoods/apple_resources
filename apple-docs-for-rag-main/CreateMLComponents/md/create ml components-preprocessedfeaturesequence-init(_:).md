

- Create ML Components
- PreprocessedFeatureSequence
-  init(\_:) 

Initializer

# init(\_:)

Creates an asynchronous sequence of stored temporal features.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
init(_ sequence: S) async throws where Feature == S.Feature, S : TemporalSequence
```

## Parameters 

`sequence`  

An asynchronous sequence of temporal features.

