

- AVFAudio
- AVAudioChannelLayout
-  init(layout:) 

Initializer

# init(layout:)

Creates an audio channel layout object from an existing one.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(layout: UnsafePointer)
```

## Parameters 

`layout`  

The existing audio channel layout object.

## Return Value

A new `AVAudioChannelLayout` object.

## Discussion

If the audio channel layout object’s tag is kAudioChannelLayoutTag_UseChannelDescriptions, this initializer attempts to convert it to a more specific tag.

## See Also

### Related Documentation

var layout: UnsafePointer&lt;AudioChannelLayout>

The underlying audio channel layout.

### Creating an Audio Channel Layout

convenience init?(layoutTag: AudioChannelLayoutTag)

Creates an audio channel layout object from a layout tag.

