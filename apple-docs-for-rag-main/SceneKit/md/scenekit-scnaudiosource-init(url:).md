

- SceneKit
- SCNAudioSource
-  init(url:) 

Initializer

# init(url:)

Initializes an audio source from the specified audio file.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(url: URL)
```

## Parameters 

`url`  

A URL locating an audio file.

## Return Value

A new audio source object.

## See Also

### Creating an Audio Source

convenience init?(named: String)

Returns the audio source associated with the specified filename.

convenience init?(fileNamed: String)

Initializes an audio source from an audio file in the application’s main bundle.

