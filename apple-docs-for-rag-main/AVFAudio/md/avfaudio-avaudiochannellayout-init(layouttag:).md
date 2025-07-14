

- AVFAudio
- AVAudioChannelLayout
-  init(layoutTag:) 

Initializer

# init(layoutTag:)

Creates an audio channel layout object from a layout tag.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init?(layoutTag: AudioChannelLayoutTag)
```

## Parameters 

`layoutTag`  

The audio channel layout tag.

## Return Value

A new `AVAudioChannelLayout` object, or `nil` if `layoutTag` is kAudioChannelLayoutTag_UseChannelDescriptions or kAudioChannelLayoutTag_UseChannelBitmap.

## See Also

### Creating an Audio Channel Layout

init(layout: UnsafePointer&lt;AudioChannelLayout>)

Creates an audio channel layout object from an existing one.

