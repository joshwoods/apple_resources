

- SceneKit
- SCNAudioSource
-  init(named:) 

Initializer

# init(named:)

Returns the audio source associated with the specified filename.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init?(named fileName: String)
```

## Parameters 

`fileName`  

The name of an audio file. If this filename has not been previously requested, the method looks for an audio file with the specified name in the application’s main bundle.

## Return Value

An audio source object.

## Discussion

This method looks in the system caches for an audio source with the specified name and returns that object if it exists. If a matching audio source is not already in the cache, this method locates the audio file with the specified name in the application’s main bundle, then creates a new audio source and caches it for reuse.

## See Also

### Creating an Audio Source

convenience init?(fileNamed: String)

Initializes an audio source from an audio file in the application’s main bundle.

init?(url: URL)

Initializes an audio source from the specified audio file.

