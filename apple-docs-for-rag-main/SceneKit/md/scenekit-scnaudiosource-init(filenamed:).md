

- SceneKit
- SCNAudioSource
-  init(fileNamed:) 

Initializer

# init(fileNamed:)

Initializes an audio source from an audio file in the application’s main bundle.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init?(fileNamed name: String)
```

## Parameters 

`name`  

The name of an audio file in the application’s main bundle.

## Return Value

A new audio source object.

## Discussion

Calling this method is equivalent to using the Bundle class to locate an audio file in the application’s main bundle and then passing the resulting URL to the init(url:) method.

## See Also

### Creating an Audio Source

convenience init?(named: String)

Returns the audio source associated with the specified filename.

init?(url: URL)

Initializes an audio source from the specified audio file.

